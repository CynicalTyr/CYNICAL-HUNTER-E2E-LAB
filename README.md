# CYNICAL-HUNTER-E2E-LAB

End-to-end testing laboratory for Cynical Hunter.

Files here hold **intentionally invalid mock keys** shaped like real tokens so detectors can match and live validators can fail. Do not put live credentials here.

- Primary fixture: `leaked_secrets.env`
- Hunter tests should scan that fixture or scope discovery to this repo.
- Live probes must reject these values (`valid_keys_found=0`). Notify must not fire on mocks.
- GitHub secret scanning may block extra provider shapes; keep the existing dummy OpenAI/Gemini/Anthropic/GitHub lines.
- If a live token was ever committed for a one-shot test, revoke it at the provider. Git history is not a safe store.

## Coffee and energy fund

If the fixture lab helped you test without live keys and you want more CynicalTyr tooling, you can chip in to the coffee and energy fund. Optional.

<a title="Donate with PayPal" href="https://www.paypal.me/ctmskm" target="_blank" rel="noopener"><img src="https://moosenet.lol/assets/images/paypal-logo.png" alt="PayPal" width="140" height="50" /></a><a title="Donate with CashApp" href="https://cash.app/$MooseMeNow" target="_blank" rel="noopener"><img src="https://moosenet.lol/assets/images/cashapp-logo.png" alt="Cash App" width="140" height="55" /></a> <a title="Donate with Venmo" href="https://venmo.com/MooseMeNow" target="_blank" rel="noopener"><img src="https://moosenet.lol/assets/images/venmo-logo-600x188.png" alt="Venmo" width="140" height="50" /></a>
