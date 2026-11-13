# Design
upload -> [video stage] -> [tts stage] -> [caption stage: word timings -> ASS] -> ffmpeg mux -> MP4
Each stage is a module with a common interface `run(job) -> job`, so stages can be swapped ("stitched").
