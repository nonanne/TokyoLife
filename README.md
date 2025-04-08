# TokyoLife

📘 Specification Document – Tokyo Student Life (React Native Version)
📌 1. Overview
Title (tentative): Tokyo Student Life
Genre: Text-based simulation + life experience + Japanese language learning
Platform: Mobile App (React Native + TypeScript)
Target Platforms: iOS / Android

Main Users:
- International students in or planning to study in Japan
- Japanese learners (JLPT N5–N3)
- Users interested in Japanese culture and daily life

🎯 2. Concept & Goals
- Provide a realistic and engaging experience of student life in Tokyo
- Enable players to make decisions on daily activities, manage money, and build relationships
- Teach useful Japanese phrases via audio clips and situational learning
- Offer multiple game modes for both realistic and casual players

🧑‍💼 3. Key Gameplay Features
✅ Daily Life Simulation
Choose how to spend each day: study, part-time job, rest, socialize, etc.

Track stats:
Money, Fatigue, Japanese Skill, Relationships, Trust, Visa Remaining Days

Living costs:
Monthly rent, Transportation fees, Optional commuter pass

✅ Social & Romantic Interactions
- Meet characters at school, part-time jobs, and dating apps
- Maintain and track relationship scores
- Unlock special events or endings based on relationship development

✅ Jobs & Gambling
Choose jobs via a Job Board

Each job has different:
Pay, Fatigue, Language gain, Chance to meet characters

Optional gambling events:
Pachinko, Horse Racing, Mahjong (non-cash rewards), with risk/reward choices

✅ Events & Bureaucracy
Simulate essential real-world actions:
- Resident registration, insurance setup, visa renewals
- Trash sorting, public transport use, bank accounts
- Some events include minigames or quizzes (e.g., garbage classification quiz)

✅ Cultural & Leisure Experiences
- Join school clubs or local community groups
- Experience karaoke, festivals, onsen, or class trips
- Encounter cultural differences and decision-based branching

🎮 4. Game Modes
Mode	Description
- Realistic	Full realism: rent, stress, bureaucracy, chance-based events
- Standard	Balanced experience, includes some costs and challenges
- Ideal	Light play: no expenses or fatigue, mainly story + learning focus

🌐 5. Language Support
Supported Languages: English, Chinese (Simplified), Spanish, French

System: react-i18next (or i18n-js)

Files: Stored in locales/ as JSON:
locales/
├── en.json
├── zh.json
├── es.json
└── fr.json

🧩 6. Key Screens
Screen	Description
- ModeSelectScreen	Choose game mode
- HomeScreen	Status overview + current day preview
- EventScreen	Main event (story text + choices + optional audio)
- JobBoardScreen	Select part-time jobs
- RelationshipScreen	View character profiles and relationship scores
- InfoScreen	Guides on bureaucracy, culture, and daily life
- ResultScreen	End summary and outcomes

⚙️ 7. Technical Stack
Functionality	Technology
UI	React Native (Expo / Bare) + TypeScript
State Management	Zustand / Redux Toolkit
Audio	expo-av / react-native-sound
Local Storage	AsyncStorage
Language Switching	react-i18next / i18n-js
Navigation	react-navigation
Animation (Optional)	react-native-reanimated or Lottie

🧪 8. Sample Game Flow
User selects “Realistic Mode”
1. Proceeds to a tutorial week
2. Starts receiving events (e.g., “Your classmate invites you to a part-time job”)
3. Makes a choice: works → earns money + fatigue → unlocks Japanese phrase
4. After several days, new features/events unlock (e.g., move, relationship, gambling)
5. Final outcome depends on choices and stats (e.g., graduation, marriage, return home)

🌱 9. Expandable Features
- JLPT mini quizzes
- Map-based Tokyo navigation
- Custom avatar & room decoration
- Seasonal events: sakura, fireworks, snow festival
- Daily challenges / Achievements
- Backend sync for multi-device progress

🔥 10. Development Priorities (Short-Term)
Priority	Feature
- High	Event system + choice processing + status tracking
- High	Language system + multi-language files
- Medium	Job board + audio-based Japanese learning
- Medium	Mode system + transport logic + housing
- Optional	Relationship profiles + event unlock conditions
