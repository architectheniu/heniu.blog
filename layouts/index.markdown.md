{{- $e := partial "heniu-ai-etykiety.html" . -}}
# Heniu.blog

{{ $e.opis }}

{{ $e.autor }}

## {{ $e.najnowsze }}

{{ range first 50 (where .Site.RegularPages.ByDate.Reverse "Section" "in" (slice "posts" "f-log" "h-log" "t-log")) -}}
- [{{ .Title }}]({{ with .OutputFormats.Get "markdown" }}{{ .Permalink }}{{ end }}) ({{ .Date.Format "2006-01-02" }})
{{ end }}
