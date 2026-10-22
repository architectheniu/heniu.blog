{{- $e := partial "heniu-ai-etykiety.html" . -}}
# {{ partial "tytul-wpisu.html" . }}

{{ $e.data }}: {{ .Date.Format "2006-01-02 15:04" }}
{{ $e.adres }}: {{ .Permalink }}
{{ $e.autor }}

---

{{ if .Params.encrypted }}{{ .Permalink }}{{ else }}{{ .RawContent }}{{ end }}
