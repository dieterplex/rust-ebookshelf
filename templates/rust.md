# {{title}}

Last updated: {{timestamp | date(format="%Y-%m-%d %H:%M")}}

#| Title | Book | Commit | Last Update
-|-------|------|--------|-------------
{% for entry in entries %}{{loop.index}} | {{entry.title}} [<i class="fa fa-book"></i>]({{entry.url}}) | [ePub <i class="fa fa-download"></i>]({{entry.path | urlencode}}) ({{entry.epub_size | filesizeformat}}) | {{entry.commit_sha | truncate(length=8, end="")}} [<i class="fa fa-git"></i>]({{entry.repo_url}}) | {{entry.last_modified | date(format="%Y-%m-%d %H:%M")}}
{% endfor %}
