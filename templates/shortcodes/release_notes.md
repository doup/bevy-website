{% import "macros/path.html" as macros %}

{% set base_path = macros::release_path(version=version, path="/release-notes/") %}
{% set release_notes_data = load_data(path=macros::path_join(path_a=base_path, path_b="/_release-notes.toml")) %}
{% for release_note in release_notes_data.release_notes %}
{% set release_note_body = load_data(path=macros::path_join(path_a=base_path, path_b=release_note.file_name)) %}

### {{ release_note.title }}

<ul class="release-feature-meta">
  {% for pr in release_note.prs %}
  <li>Authors: {{ pr.authors | join(sep=", ")}}</li>
  <li><a href="{{ pr.url }}">{{ pr.title }}</a></li>
  {% endfor %}
</ul>

{{ release_note_body }}

{% endfor %}
