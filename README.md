# IELTS Listening Practice — Cambridge 17–19

This repository contains 12 complete Listening tests: four each from Cambridge IELTS 17, 18 and 19.

## The only manual file setup you need

You do **not** need a separate audio folder for each test.

There are only three audio folders:

```text
audio/
├── cambridge-17/
├── cambridge-18/
└── cambridge-19/
```

Put all 16 Cambridge 17 audio files in `audio/cambridge-17/`, all 16 Cambridge 18 audio files in `audio/cambridge-18/`, and all 16 Cambridge 19 audio files in `audio/cambridge-19/`.

Keep the filenames exactly as they are. The website already knows which file belongs to which test and Part.

### Cambridge 17
Copy all 16 files into: `audio/cambridge-17/`

- Test 1 Part 1: `IELTS17_t1_audio1 [@cambridge_library].mp3`
- Test 1 Part 2: `IELTS17_t1_audio2 [@cambridge_library].mp3`
- Test 1 Part 3: `IELTS17_t1_audio3 [@cambridge_library].mp3`
- Test 1 Part 4: `IELTS17_t1_audio4 [@cambridge_library].mp3`
- Test 2 Part 1: `IELTS17_t2_audio1 [@cambridge_library].mp3`
- Test 2 Part 2: `IELTS17_t2_audio2 [@cambridge_library].mp3`
- Test 2 Part 3: `IELTS17_t2_audio3 [@cambridge_library].mp3`
- Test 2 Part 4: `IELTS17_t2_audio4 [@cambridge_library].mp3`
- Test 3 Part 1: `IELTS17_t3_audio1 [@cambridge_library].mp3`
- Test 3 Part 2: `IELTS17_t3_audio2 [@cambridge_library].mp3`
- Test 3 Part 3: `IELTS17_t3_audio3 [@cambridge_library].mp3`
- Test 3 Part 4: `IELTS17_t3_audio4 [@cambridge_library].mp3`
- Test 4 Part 1: `IELTS17_t4_audio1 [@cambridge_library].mp3`
- Test 4 Part 2: `IELTS17_t4_audio2 [@cambridge_library].mp3`
- Test 4 Part 3: `IELTS17_t4_audio3 [@cambridge_library].mp3`
- Test 4 Part 4: `IELTS17_t4_audio4 [@cambridge_library].mp3`

### Cambridge 18
Copy all 16 files into: `audio/cambridge-18/`

- Test 1 Part 1: `C 18 section1-part1[@cambridge_library].mp3`
- Test 1 Part 2: `C 18 section1-part2[@cambridge_library].mp3`
- Test 1 Part 3: `C 18 section1-part3[@cambridge_library].mp3`
- Test 1 Part 4: `C 18 section1-part4[@cambridge_library].mp3`
- Test 2 Part 1: `C 18 section2-part1[@cambridge_library].mp3`
- Test 2 Part 2: `C 18 section2-part2[@cambridge_library].mp3`
- Test 2 Part 3: `C 18 section2- part3 [@cambridge_library].mp3`
- Test 2 Part 4: `C 18 section2- part4[@cambridge_library].mp3`
- Test 3 Part 1: `C 18 section3 part1 [@cambridge_library].mp3`
- Test 3 Part 2: `C 18 section3 part2[@cambridge_library].mp3`
- Test 3 Part 3: `C 18 section3 part3[@cambridge_library].mp3`
- Test 3 Part 4: `C 18 section3 part4[@cambridge_library].mp3`
- Test 4 Part 1: `C 18 section4 part1[@cambridge_library].mp3`
- Test 4 Part 2: `C 18 section4 part2[@cambridge_library].mp3`
- Test 4 Part 3: `C 18 section4 part3[@cambridge_library].mp3`
- Test 4 Part 4: `C 18 section4 part4[@cambridge_library].mp3`

### Cambridge 19
Copy all 16 files into: `audio/cambridge-19/`

- Test 1 Part 1: `T1 P1 [@cambridge_library].mp3`
- Test 1 Part 2: `T1 P2 [@cambridge_library].mp3`
- Test 1 Part 3: `T1 P3 [@cambridge_library].mp3.mp3`
- Test 1 Part 4: `T1 P4 [@cambridge_library].mp3`
- Test 2 Part 1: `T2 P1 [@cambridge_library].mp3`
- Test 2 Part 2: `T2 P2 [@cambridge_library].mp3`
- Test 2 Part 3: `T2 P3 [@cambridge_library].mp3`
- Test 2 Part 4: `T2 P4 [@cambridge_library].mp3`
- Test 3 Part 1: `T3 P1 [@cambridge_library].mp3`
- Test 3 Part 2: `T3 P2 [@cambridge_library].mp3`
- Test 3 Part 3: `T3 P3 [@cambridge_library].mp3`
- Test 3 Part 4: `T3 P4 [@cambridge_library].mp3`
- Test 4 Part 1: `T4 P1 [@cambridge_library].mp3`
- Test 4 Part 2: `T4 P2 [@cambridge_library].mp3`
- Test 4 Part 3: `T4 P3 [@cambridge_library].mp3`
- Test 4 Part 4: `T4 P4 [@cambridge_library].mp3`


## Important

The MP3 files themselves are not included in this ZIP. Everything else is already organised.

The website includes:
- 12 Listening tests
- 40 questions per test
- automatic marking
- accepted answer variants
- persistent progress with `localStorage`
- a 1–40 question navigator
- sequential Parts
- one-play client-side audio behaviour
- raw score out of 40
- answer review after submission
- no student-visible reset button

Client-side one-play control is not DRM. A technically knowledgeable user could bypass it by changing browser storage, source code or media requests.

## Run locally

Because the test data are loaded with JavaScript, serve the folder through HTTP instead of opening `index.html` directly.

```bash
cd ielts-listening
python -m http.server 8000
```

Then open `http://localhost:8000/`.

## Simplified repository structure

```text
ielts-listening/
├── index.html
├── test.html
├── README.md
├── assets/
├── data/
├── questions/
└── audio/
    ├── audio-map.json
    ├── cambridge-17/
    ├── cambridge-18/
    └── cambridge-19/
```

You only need to manually add files inside the three `audio/cambridge-XX/` folders.
