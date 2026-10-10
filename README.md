# Plant Disease Detector (React + Teachable Machine)

Upload a leaf image and the app shows **only the single predicted label**.

## Run it

Requires Node.js 18+.

```bash
npm install
npm start
```

(`npm run dev` does the same thing.)

Open the URL shown in the terminal (usually http://localhost:5173).

## Production build

```bash
npm run build
npm run preview
```

## Using a different model

Open `src/App.jsx` and change the `MODEL_URL` constant at the top:

```js
const MODEL_URL = "https://teachablemachine.withgoogle.com/models/-iJgVAU9z/";
```

## Notes

- TensorFlow.js and the Teachable Machine image library are loaded from the jsDelivr CDN in `index.html` (same as the Teachable Machine export code), so an internet connection is needed.
- The result is a preliminary prediction and not a confirmed agricultural diagnosis.
