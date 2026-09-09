# CYNICAL-HUNTER-E2E-LAB

End-to-end testing laboratory for Cynical Hunter.

Files here hold **intentionally invalid mock keys** shaped like real tokens so detectors can match and live validators can fail. Do not put live credentials here.

- Primary fixture: `leaked_secrets.env`
- Hunter tests should scan that fixture or scope discovery to this repo.
- Live probes must reject these values (`valid_keys_found=0`). Notify must not fire on mocks.
- GitHub secret scanning may block extra provider shapes; keep the existing dummy OpenAI/Gemini/Anthropic/GitHub lines.
- If a live token was ever committed for a one-shot test, revoke it at the provider. Git history is not a safe store.
