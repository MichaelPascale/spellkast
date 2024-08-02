# spellkast
This software supports my personal notetaking style by combining notes either typed or handwritten on paper or tablet. The output is a directory of markdown files named by date. I begin all of my notes, regardless of format, with a standard header including the datetime and topic (e.g. "2024-07-31 11:00 EDT Lab meeting").

## Handwritten

### Index Cards

Multiple index cards can be scanned at once on a flatbed scanner (or with a photo). I use OpenCV to segement and rotate the index cards. Text is extracted with Tesseract.

### Notebooks

Handwritten notes are scanned to PDF and extracted with Tesseract.

### ReMarkable

The ReMarkable e-paper tablet supports handwriting-to-text. I use the (unofficial) ReMarkable Cloud API to extract text from recent notes.

## Typed

### LogSeq
LogSeq journal entries are extracted directly as Markdown.

### Text Files (Markdown)
Other text files are extracted directly. Markdown headers for date-time and topic are added automatically if they do not exist.
