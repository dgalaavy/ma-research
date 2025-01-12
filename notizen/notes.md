# Notizen

## Einleitung

### Motivation

- Mamba als neues Modell im NLP Kontext
  - Konkurrent zu Transformern ohne Attention und mit
    weniger Parametern?
- Verschiedene Ansätze für Vision Mamba
- Edge TPU als Beschleuniger der Interferenz in Embedded Devices
  wie dem Raspberry Pi (5)
- Anwendung: Gefäß-Segmentierung in Netzhautbildern

### Technische Herausforderung

- Edge TPU hat nur beschränktes Operationsset,
  das genutzt werden kann
- Edge TPU kann nur int8 modelle
- Mamba Modelle lassen sich also nicht so leicht übertragen

### Zielsetzung

- Mamba Modell zur Image Segmentierung, das auf der Coral
  Edge TPU läuft, präzise genug ist und wenig Latenz zeigt

## Theoretischer Hintergrund

### Edge TPU

- Google
- Tf Lite
- Debian System
- unterstützte Operatoren
- Quantisierung nach dem Training
- https://coral.ai/docs/edgetpu/models-intro/#model-requirements

### Mamba

- Idee und Abgrenzung zu Transformer

### Vision Mamba

- verschiedene Ansätze
- Operatoren, die verwendet werden?

### Daten

- Wo kommen Daten her?
- Was zeigen die Daten?
- Beispiel

### Metriken???

## Methoden

- Vision Mamba Modell Parametrisiert geschrieben
- Hyperparameter Tuning

## Evaluation

- Vergleich der Laufzeit / Throughput auf verschiedenen Geräten
  - PI
  - PI + TPU
  - CPU (Rechner / Laptop)
  - GPU (Rechner / Laptop)
  - verschiedene Tests, Anzahl etc.
    -> qualitativ und quantitativ
- Vergleich der gewählten Metrik auf den oben genannten Geräten
  (post-quantisiertes Modell vor und nach Quantisierung)


