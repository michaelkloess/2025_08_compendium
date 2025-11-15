Einfach Baumstruktur in Visual Studio Code Terminal im Projekt erzeugen - Ergebnis wird im Terminal ausgegeben:

find . -type d \( -name ".git" -o -name "node_modules" \) -prune -o -print | sed -e 's/[^-][^\/]*\//   |/g' -e 's/|\([^ ]\)/|-- \1/'

Alternative: Ergebnis in einer Markdown Datei speichern, die im Projekt abgelegt wird - Dateiname wird am Ende definiert "> struktur.md"

(echo '```'; find . -type d \( -name ".git" -o -name "node_modules" \) -prune -o -print | sed -e 's/[^-][^\/]*\//   |/g' -e 's/|\([^ ]\)/|-- \1/'; echo '```') > struktur.md
