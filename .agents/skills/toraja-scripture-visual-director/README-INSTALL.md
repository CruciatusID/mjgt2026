# Toraja Scripture Visual Director — Antigravity IDE installation

## Install
1. Extract ZIP.
2. Copy the entire folder `toraja-scripture-visual-director` into the skill folder recognized by your Antigravity installation. A common workspace location for agent skills is `.agent/skills/toraja-scripture-visual-director/` (confirm against your installation's supported skill discovery path). Keep `SKILL.md`, `references/`, `templates/`, and `examples/` relative to it.
3. Restart/reload agent context or skill discovery as needed. Do not flatten the folder: internal relative paths matter.
4. Put your weekly sermon `.md` in the project or attach/provide its absolute file path to agent.

## First test command (copy to Antigravity chat)
"Gunakan skill `toraja-scripture-visual-director`. Baca file MD tema Gereja Toraja tanggal 4 Oktober 2026 yang saya berikan. Jalankan hanya Stage A. Analisis tujuan, bacaan, korelasi dan pokok khotbah; buat tepat 3 konsep ilustrasi 4:3 painterly 3D yang layak di-expand ke 16:9, masing-masing satu adegan utuh, tanpa split-screen atau teks. Berikan skor, alasan, serta rekomendasi. Jangan render gambar atau membuat prompt final sampai saya memilih."

## Second test after choosing
"Saya pilih konsep [nomor]. Lanjut Stage B. Buat prompt master 4:3, prompt outpainting simetris ke 16:9 dengan area 4:3 terkunci, dan prompt judul bahasa Indonesia persis sesuai MD pada background hitam murni untuk pemisahan manual. Berikan juga instruksi tipografi presisi dan QA checklist."

## Workflow behavior
- Stage A produces concept report only.
- User selects concept.
- Stage B produces production prompts and title design spec.
- Image generation and QA occur only when requested and tools/images are actually available.
- Don't claim rendered outputs where only prompts exist.

## Assets
Example source is included at `examples/source-weekly-theme-2026-10-04.md` for reproducible testing. The test concept interpretation is at `examples/2026-10-04-concept-smoke-test.md`.
