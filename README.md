# Training Tracker

A single-page tracker for a 12-week plan: cycling three days a week and lifting two days a week, aimed at general fitness with a knee-friendly start.

Everything lives in one file, `index.html`. There is nothing to install and no server.

## What it does

- **12-week plan.** Week-by-week cycling targets (easy rides, Thursday intervals, a Sunday long ride) and two lifting sessions.
- **Heart-rate targets.** Easy rides at 125–145 bpm, interval blocks at 150–160 bpm.
- **Log your sessions.** Enter time, distance, average and max heart rate for each ride. Average speed is calculated for you.
- **Log your lifts.** Enter the weight and reps for every set. Use **Log as planned** to fill in a whole exercise in one tap.
- **Warm-up sets.** Each barbell lift shows warm-up sets calculated from its working weight, plus the plates to load on each side.
- **Weights that adjust.** If you finish every set at the target reps, next week's weight goes up by the planned step. If you miss reps, or flag your knee, the weight holds.
- **Easy weeks.** Weeks 4, 8 and 12 keep the weights but drop one set per lift, with shorter rides.
- **Knee check and notes.** A weekly check-in with a reminder to hold weights if you report swelling or instability.

## Using it

Open the page and use the bottom tabs:

| Tab | What it shows |
|---|---|
| This week | The current week's rides and lifts, with boxes to log them |
| All 12 weeks | The full plan, with what you actually lifted shown next to each target |
| Guide | Heart-rate zones, lifting rules, knee notes and backup tools |

Tap a week number at the top to jump between weeks.

## Where your data is stored

Your log is saved **in your browser on the device you use**, under this page's address. It is not uploaded to GitHub or anywhere else, and nobody else can see it.

This means:

- Opening the page in a different browser, or on a different device, shows an empty tracker.
- Clearing the browser's site data erases your log.
- Changing the page's address (for example by renaming the repository) starts you with an empty log.

### Backing up

Use the **Your data** section in the Guide tab:

- **Back up (JSON)** saves your whole log to a file. Do this about once a week.
- **Restore from backup** loads a backup file. It replaces the log on the current device, so use the newest backup.
- **Download CSV** exports your log as a spreadsheet-friendly file.

Each backup is a full copy, so only the most recent one matters. Browsers add `(1)`, `(2)` and so on to repeated downloads, so delete old ones now and then.

## Updating the page

To change the page, replace `index.html` in this repository with a new version (same file name) and commit. Your logged numbers stay, because the page's address does not change.

## Hosting on GitHub Pages

1. Create a public repository and add `index.html` to the main folder.
2. Go to **Settings**, then **Pages**.
3. Under "Build and deployment", set Source to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, and save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Equipment assumptions

- A 20 kg Olympic barbell.
- One pair each of 1.25, 2.5, 5, 10, 20 and 25 kg plates, so weights move in 2.5 kg steps.
- A squat rack with safety pins, a bench and adjustable dumbbells.

Plate loading assumes one plate of each size per side. Heavy collars add weight.

## Notes and limits

- Weeks 7–12 start from projected weights and adjust as you log.
- Only the six barbell lifts adjust automatically. Dumbbell and bodyweight exercises are for you to choose.
- Heart-rate zones are based on a highest recorded heart rate of 176 bpm and will need adjusting if yours differs.
- This is a personal training plan, not medical advice. If you notice swelling, instability or pain that lingers after training, stop increasing load and see a physiotherapist.
