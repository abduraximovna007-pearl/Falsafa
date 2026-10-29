# Stitch prompt: "Falsafa Bellashuvi"

Design and build a responsive single-page website for a philosophy quiz game called "Falsafa Bellashuvi" (Philosophy Showdown). The interface text must be in Uzbek (Latin script). Use the exact texts provided below.

## Visual direction

- Elegant, calm, intellectual. Premium but not flashy, and not boring or corporate.
- Palette: warm ivory background (`#F6F1E7`), deep ink text (`#1F2A36`), muted terracotta accent (`#B5654A`), soft sage secondary (`#8FA596`), with light sand surfaces (`#EDE4D3`) for cards. Avoid neon, harsh black/white contrast, and heavy gradients. Keep it easy on the eyes for long sessions.
- Typography: a refined serif for headings (e.g. Playfair Display or Cormorant), a clean sans-serif for body text (e.g. Inter or Manrope). Generous line height and whitespace.
- Subtle motion: soft fade and slide transitions only. No flashy effects.
- Avoid generic template look: use thoughtful spacing, thin dividers, and quote marks as decorative elements.

## Page structure

### 1. Header / Hero

- Big title: "Falsafa Bellashuvi"
- Short, engaging paragraph about what philosophy is:

> Falsafa — donolikka bo'lgan muhabbat degani. Bu so'z qadimgi yunon tilidagi 'philo' (sevgi) va 'sophia' (donolik) so'zlaridan kelib chiqqan. Falsafa bizga savol berishni o'rgatadi: nima haqiqat, nima adolat, inson nima uchun yashaydi?

- Primary button: "Boshlash"

### 2. Famous thinkers carousel (swipe / slider)

- 9 cards, one visible at a time, navigable by swipe, arrows, and dots.
- Each card contains: a photo slot (large, rounded corners, 4:5 ratio), the person's name, and their quote in quotation marks.
- Use image placeholders that I will replace with my own uploaded photos. Clearly mark the placeholder slots with an easily replaceable image element.
- Content (in this order):
  1. Lao Szi — "Boshqalarni biluvchi – oqil, o‘zini biluvchi – donishmanddir."
  2. Protagor — "Inson barcha narsalar mezonidir."
  3. Suqrot — "O‘z-o‘zingni angla va shu orqali dunyoni anglaysan."
  4. Rene Dekart — "Inson – fikrlovchi narsadir."
  5. Jan-Pol Sartr — "Inson – odamzod kelajagidir."
  6. Ibn Sino — "Inson boshqa barcha hayvonot olamidan so‘zi, tili va aqli, tafakkur qilishi bilan farq qiladi."
  7. Artur Shopengauer — "Inson – nuqsonli mavjudot hamda u tabiat xalturasidir."
  8. Konfutsiy — "O‘zingga ravo ko‘rmagan narsani o‘zgaga ham munosib ko‘rma."
  9. Iso at-Termiziy — "Qayerda bilim va ilmga e’tibor kamaysa, o‘sha yerda odamlar axloqan tubanlasha boshlaydilar."

### 3. Participant picker

- Section title: "Ishtirokchini tanlang"
- Pool of 18 participants (exact names, each appears once per game):
  Gulsevar, Rano, Sabina, Saodat, Javohir, Jafarbek, Sarvinoz, Nodira, Madina, Shahina, Xurshida, To'lqin, Shohjahon, Shahzoda, Zarina, Ruhshona, Suhrob, Ulug'oy
- A "Tasodifiy tanlash" (Random pick) button. On click: a short shuffle animation over the remaining names, then the selected name is revealed. Already-played names are removed from the pool.
- Show a counter: "Qatnashdi: X / 18"

### 4. Test (3 questions per participant)

- Show the participant's name and a live timer that starts with the first question.
- Each question: one quote from the 9 thinkers, shown in quotation marks, and 3 author options as big tappable buttons. Choose randomly from the 9 thinkers, with no repeated quote within the same participant's test.
- After each answer, show brief feedback: correct or incorrect.
- Track score (0–3) and total time.

### 5. Result stickers (shown after the 3 questions)

- 3/3: "Zo'r!" sticker with a big smile and celebration icon.
- 2/3: "A'lo!" sticker with a happy smile.
- 1/3: "Yaxshi" sticker with a neutral-positive face.
- 0/3: "Yomon" sticker with a sad, disappointed face and a slightly wobbly shape. Keep it cute, not mean.
- Stickers are flat, illustrated badges in the palette above. Each shows the participant's name and score.
- Button: "Keyingi ishtirokchi" (Next participant) if the pool is not empty, otherwise go to results.

### 6. Bonus task (only for participants who scored 0/3)

- Show one quote from the 9 thinkers and 3 author options. Use a different quote than the test ones when possible.
- If correct: show a "Barakalla!" message with celebration styling, then a "Keyingisini tanla" (Pick next) button that returns to the participant picker.
- If incorrect: show a gentle encouragement message and allow one retry.

### 7. Final leaderboard (after all 18 participants have played)

- Title: "Bugungi g'oliblar"
- Ranking rules: 1) higher score first, 2) for equal scores, faster total time first.
- Show top 3 with a podium-style layout: 1st, 2nd, 3rd place, with name, score, and time.
- Show a "Sovg'a" (Prize) label under each winner.
- Button: "Qayta boshlash" (Restart).

## Technical notes

- Single-page app, responsive for mobile and desktop.
- Store game state in memory during the session: participant pool, results, timers, and scores.
- Clean, accessible markup: good color contrast, keyboard navigation, and labeled buttons.
- Placeholder images should use a neutral sand-colored box until replaced.

---

## Qo'shimcha maslahatlar

- Rasmlarni yuklaganingizda, Stitch'ga "Replace the 9 image placeholders with the uploaded photos in the same order as the carousel cards" deb ayting.
- Agar natija juda ko'p ranglı chiqsa, "Reduce the palette to 3 colors, keep the ivory background" deb tuzatishni so'rang.
- Dizayn tayyor bo'lgach, stikerlarni alohida so'rov bilan yaxshilash mumkin.
