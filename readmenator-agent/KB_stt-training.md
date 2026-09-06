# Subsystem: stt-training

## micro/stt-training/config.sh
- Layer: infrastructure
- Doc: Shared configuration for the STT training pipeline. Sourced by run_all.sh and safe to source in your own shell: . ./conf
- Language: sh

## micro/stt-training/run_all.sh
- Layer: utility
- Doc: End-to-end pipeline: synthesize -> mine -> extract -> train -> evaluate -> export.  Edit words.txt first, then run:  ./r
- Language: sh
