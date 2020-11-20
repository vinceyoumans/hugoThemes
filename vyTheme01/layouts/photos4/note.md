<div class="jumbotron jumbotron-fluid">
  <div class="container">
    {{/*  <h1 class="display-4">Fluid jumbotron</h1>  */}}
    {{/*  <h1 class="display-4"> {{ .Weight }} - {{ .Title | markdownify }}</h1>
    <p class="lead">  {{ .Params.Description | markdownify }} </p>  */}}

      <time class="post-date"
        datetime="{{ .Date.Format "2006-01-02T15:04:05Z07:00" | safeHTML }}">{{ .Date.Format "Jan 2, 2006" }}
      </time>
      {{/*  <br>
      <h4>{{ .Params.Description | markdownify }}</h4>  */}}
      {{/*  <h3>use this link to reference in your emails and other Etext</h3>  */}}
      <h3><a href="{{ .Permalink | relURL }}" class="card-link">PERMA LINK</a></h3>

      {{ if .Params.tags }}
      <div class="blog-tags">
        {{ range .Params.tags }}
          <a href="{{ $.Site.LanguagePrefix | absURL }}/tags/{{ . | urlize }}/">{{ . }}</a>&nbsp;
        {{ end }}
      </div>
    {{ end }}

  </div>
</div>



<div class="jumbotron jumbotron-fluid">
  <div class="container">
    {{/*  <h1 class="display-4">Fluid jumbotron</h1>  */}}
    <h1 class="display-4"> {{ .Weight }} - {{ .Title | markdownify }}</h1>
    <p class="lead">  {{ .Params.Description | markdownify }} </p>

      <time class="post-date"
        datetime="{{ .Date.Format "2006-01-02T15:04:05Z07:00" | safeHTML }}">{{ .Date.Format "Jan 2, 2006" }}
      </time>
      {{/*  <br>
      <h4>{{ .Params.Description | markdownify }}</h4>  */}}
      {{/*  <h3>use this link to reference in your emails and other Etext</h3>  */}}
      <h3><a href="{{ .Permalink | relURL }}" class="card-link">PERMA LINK</a></h3>

      {{ if .Params.tags }}
      <div class="blog-tags">
        {{ range .Params.tags }}
          <a href="{{ $.Site.LanguagePrefix | absURL }}/tags/{{ . | urlize }}/">{{ . }}</a>&nbsp;
        {{ end }}
      </div>
    {{ end }}

  </div>
</div>

{{/*  <div class="container">
  <div class="card">
    <div class="card-header bg-info">
      <h1>{{ .Weight }} - {{ .Title | markdownify }}</h1>
      <time class="post-date"
        datetime="{{ .Date.Format "2006-01-02T15:04:05Z07:00" | safeHTML }}">{{ .Date.Format "Jan 2, 2006" }}
      </time>
      <br>
      <h4>{{ .Params.Description | markdownify }}</h4>
      <h3>use this link to reference in your emails and other Etext</h3>
      <h3><a href="{{ .Permalink | relURL }}" class="card-link">PERMA LINK</a></h3>
    </div>
  
    {{ if .Params.tags }}
    <div class="blog-tags">
      {{ range .Params.tags }}
        <a href="{{ $.Site.LanguagePrefix | absURL }}/tags/{{ . | urlize }}/">{{ . }}</a>&nbsp;
      {{ end }}
    </div>
  {{ end }}

  </div>
</div>
<br>
<div class="container">
  <h3>{{ .Content }}</h3>
  {{ .Content | markdownify }}
</div>  */}}


