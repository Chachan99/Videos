# CTrackerGPS – Video publicitario 10 s (9:16)

**Uso:** subir `astronauta_ctrackergps.png` (imagen de referencia) como *first frame / image-to-video* y pegar el prompt.
Herramientas recomendadas: Veo 3 / Veo 3.1 (genera voz y música), Kling 2.x o Hailuo (si no generan audio, ver "Plan B").

## Prompt maestro (inglés, rinde mejor en los modelos)

```
Premium 3D animated commercial, Pixar-style futuristic, cinematic lighting, vertical 9:16, 10 seconds.
Use the reference image as the exact main character: a small white robotic astronaut with turquoise-blue
details, glossy helmet, dark digital visor, CTRACKER logos on the helmet and chest panel. Do NOT alter his
design, colors or logos.

0-2s: He comes to life, waves with his right hand, smiles through the visor glow, slight head tilt.
Camera: slow push-in.
2-5s: He speaks directly to the viewer in Colombian Spanish, expressive natural gestures with both arms,
head and body, friendly and trustworthy. Holographic screens appear floating beside him: a 3D car.
5-8s: Holographic GPS map with a pulsing real-time location pin, then a security alert notification.
Camera: gentle orbit.
8-10s: He points confidently at the viewer, thumbs-up, holographic shield glows. Camera settles on hero shot.

Background: dark blue tech environment, digital planet Earth, satellite connection lines, turquoise lights,
soft volumetric glow. Smooth professional camera moves. Modern holographic effects.

Dialogue (lip-synced, Colombian Spanish accent, young male, charismatic, energetic, friendly, clear diction,
modern commercial tone): "¡Hola! Soy tu amigo de CTrackerGPS. Conoce dónde está tu vehículo en tiempo real,
recibe alertas y disfruta de mayor tranquilidad. ¡Con CTrackerGPS tienes el control!"

Music: soft futuristic electronic background, low volume under the voice.
```

**Negative prompt:** subtitles, on-screen text, captions, extra logos, redesign of the astronaut, color change,
distorted logo, deformed hands, extra fingers, camera shake, watermark, low quality.

## Plan B (si el modelo no genera voz sincronizada)
1. Generar el video **mudo** con el prompt (quitar la línea de Dialogue).
2. Voz: ElevenLabs → voz masculina joven, idioma Spanish, acento Colombia (Voice Library, filtro "Colombian").
   Stability ~35 %, Similarity ~80 %, Style ~40 %. Empezar la locución a 0.5 s (≈27 palabras en ≈9 s: ritmo ágil).
3. Sincronía labial: Hedra, HeyGen, Sync Labs o Kling Lip-Sync con el video + audio.
4. Música: Suno/Udio ("soft futuristic electronic, corporate tech, 100 bpm, instrumental") a -18 dB bajo la voz.
5. Escalar a 4K (Topaz Video AI o Magnific/Upscale del propio modelo) y montar en CapCut/DaVinci.

## Consejos
- Si el logo del casco se deforma, generar 2 clips de 5 s (usar el último frame del primero como inicio del segundo).
- Si salen textos o subtítulos, reforzar el negative prompt y no pedir "pantalla con texto" en los hologramas.
- Exportar H.264, 2160x3840, 30 fps.
