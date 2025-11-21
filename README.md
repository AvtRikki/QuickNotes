# QuickNotes

QuickNotes is a lightweight, fast, and AI‑powered note‑taking application designed for simplicity and speed. It features seamless text editing, AI autocompletion, drag‑and‑drop image upload, and Firebase Storage integration.

## Features

- **Fast and minimal UI** for distraction‑free writing
- **AI Completion (Shift + A)** using Vercel AI SDK
- **Image Uploads** via drag & drop, clipboard paste, or URL — stored in Firebase Storage
- **Modern editor** powered by Tiptap
- **Responsive layout** optimized for desktop and mobile
- **Clean architecture** suitable for extension and customization

## Tech Stack

- **Next.js / React**
- **TypeScript**
- **Tiptap** (Rich Text Editor)
- **Firebase Storage** (file uploads)
- **Vercel AI SDK** (AI completions)
- **TailwindCSS** (optional)

## Installation

```bash
git clone https://github.com/AvtRikki/QuickNotes
cd QuickNotes
npm install
```

Create `.env.local`:

```
OPENAI_API_KEY=your_key_here

NEXT_PUBLIC_FIREBASE_API_KEY=...
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=...
NEXT_PUBLIC_FIREBASE_PROJECT_ID=...
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=...
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=...
NEXT_PUBLIC_FIREBASE_APP_ID=...
```

## Development

```bash
npm run dev
```

App runs at:

```
http://localhost:3000
```

## AI Autocomplete

Press **Shift + A** inside the editor to trigger AI completion. The last ~30 words are used as context.

## Project Structure

```
/app
  /api/completion
  /notes
/components
/lib
  firebase.ts
  uploadFileToFirebase.ts
```

## Future Improvements

- Note syncing across devices
- Full‑text search
- Tagging system
- Offline mode
- Collaborative editing

## License

MIT License.
