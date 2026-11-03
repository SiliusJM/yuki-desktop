# Yuki V2 — Registro público de 41 incidencias

**Estado: desarrollo en pausa.** Transcripción pública de los identificadores y estados técnicos documentados al archivar el proyecto; se omiten asignaciones internas y detalles privados. Los estados históricos no constituyen aceptación física.

| ID | Incidencia | Estado técnico histórico documentado |
| --- | --- | --- |
| YF-01 | Audible whine in voice output | OPEN / ACOUSTIC CAUSE UNKNOWN. H13 physical whine persists. H14 generated Pocket waveform has no clipping; this does not clear whine or Windows playback. |
| YF-02 | Slow voice startup | PARTIAL. H14 process-to-Pocket-ready was 47.5 s under concurrent validation/I/O; model initialization is distinct from first PCM. Installed cold startup cause remains unisolated. |
| YF-03 | First-response latency | PARTIAL. H14 generated phrases reached first PCM at 275 ms first / 98 ms warm. Browser first playback and physical response latency remain NOT MEASURED. |
| YF-04 | First output may use the wrong speaker | TECHNICAL CORRECTION / PHYSICAL FAILURE OPEN. H14 preserves both prior sinks and stored preference on failed explicit selection. The cause of the H13 Windows sink rejection remains UNKNOWN. |
| YF-05 | RVC controls can race across busy operations | TECHNICAL PASS. H14 additionally captures the requested profile before awaiting recording cancellation, preventing a later control value from replacing it; directed regression passes. |
| YF-06 | Cold RVC preparation and tuning latency | PARTIAL. A01 bounded integrity hashing and retained preparation stages; cold real-model GUI measurement is outstanding. |
| YF-07 | Complete microphone, speaker, avatar and voice flow | BLOCKED / H13 PHYSICAL FAILURE OPEN. H14 corrects reproduced software orderings; exact H13 STT/cancellation cause and complete installed flow are not proven. No H14 installer exists. |
| YF-08 | Long typed answers may be silent | TECHNICAL PASS. A01 retains the full written answer and uses one brief spoken acknowledgement above the chunk limit; audible UX remains unaccepted. |
| YF-09 | Raw tool/function markers may appear in streamed text | TECHNICAL PASS. C01 implements the bounded conversation-marker handling and directed coverage. |
| YF-10 | Local-time intent and presentation can diverge | IMPLEMENTED / HUMAN ACCEPTANCE PENDING. D01 routes exact local-time questions through the local time tool; real-device presentation is not accepted. |
| YF-11 | Google Tasks due-date presentation is ambiguous | IMPLEMENTED / HUMAN ACCEPTANCE PENDING. D01 presents pending titles and due dates only; real-account presentation remains unaccepted. |
| YF-12 | YouTube comment requests and authorship context | TECHNICAL PASS. C01 records classifier/context corrections; live user-data acceptance is not established. |
| YF-13 | YouTube channel changes require unclear restart context | TECHNICAL PASS / HUMAN ACCEPTANCE PENDING. C01 records contextual restart handling; user-facing flow has not been accepted. |
| YF-14 | Error or interruption may leave the UI in “Processing” | TECHNICAL PASS. C01 records terminal-state handling and directed error/cancel coverage. |
| YF-15 | Default response style may be too verbose | IMPLEMENTED / HUMAN ACCEPTANCE PENDING. D01 prefers concise Spanish while preserving explicit detail and selected preferences. |
| YF-16 | Technical-name pronunciation | PARTIAL. D01 added text-verified proposals; acoustic quality is unverified. |
| YF-17 | Windows and newer names pronunciation coverage | PARTIAL. D01 leaves Windows and some names for acoustic review; no broad TTS change was made. |
| YF-18 | Character/profile controls are visually fragmented | PARTIAL. E01 contains desktop UX changes; the visual flow still needs acceptance. |
| YF-19 | Legacy personality and character profile surfaces overlap | PARTIAL. E01 contains scoped UI changes; no full visual acceptance is recorded. |
| YF-20 | Normal character image import, crop and persistence | HISTORICALLY ACCEPTED for normal Settings import, framing, Save/Cancel and restart restoration. Preserve that contract. |
| YF-21 | Legacy character image import does not fully meet the user request | PARTIAL. Normal Settings image behavior has historical acceptance, but legacy character image import remains incomplete; this is not closed by E01. |
| YF-22 | VRM caption sizing and placement | PARTIAL. E01 adjusts the caption surface; visual acceptance in a real window remains pending. |
| YF-23 | Global and avatar hotkey behavior | HISTORICALLY ACCEPTED for the existing manager, allowlist and conflict handling. Preserve the contract. |
| YF-24 | Provider setup can silently retain MockAIProvider | TECHNICAL PASS. B01 fails closed and exposes effective provider state through directed coverage. |
| YF-25 | Diagnostics can imply remote health without a recent check | TECHNICAL PASS after H14 repair. IPC now accepts the bounded availability/runtime fields actually emitted by B01; invalid enums and unknown credential fields remain rejected. |
| YF-26 | Credential presence can be mistaken for effective provider readiness | TECHNICAL PASS after H14 repair. Effective-provider metadata now crosses the validated IPC boundary; no provider authorization or credential handling was broadened. |
| YF-27 | Provider-native search support and consent boundaries | PARTIAL. D01 documents supported adapters and limits; unsupported model/provider combinations remain unsupported. |
| YF-28 | OmniRoute, Kiro and ChatGPT web search lifecycle | BLOCKED / UNVERIFIED / NOT IMPLEMENTED. Provider contracts, terms, authorization and runtime behavior are not established. No cookie reuse, bypass or unsupported adapter was added. |
| YF-29 | Optional desktop shortcut in the installer | IMPLEMENTATION PRESENT / INSTALLER ACCEPTANCE PENDING. E01 changes are included; no physical installer acceptance is claimed. |
| YF-30 | NSIS finish-page launch checkbox and startup | IMPLEMENTATION PRESENT / CURRENT INSTALLER ACCEPTANCE PENDING. H03 fix is retained, current source contract tests pass, NSIS v3.04 exists, and existing H12 PE/config verification passes. No H14 NSIS compile or install/uninstall was performed. |
| YF-31 | Release notes and public release/tag provenance | RELEASE BLOCKER. The installer hook points to `https://github.com/SiliusJM/yuki-desktop/releases/tag/v${VERSION}`. The source candidate version is `0.2.0-stable.4`; no public tag or published release is claimed or verified. Installer/release-note acceptance remains pending. |
| YF-32 | Historical .3→.4 upgrade, settings retention, GUI and taskbar icon | HISTORICALLY ACCEPTED as recorded in the master audit; this is not acceptance of the current consolidation. |
| YF-33 | Full-suite evidence for the current consolidated candidate | H15 FULL-SUITE PASS: one final run at d6406c8 has 1,929 PASS / 0 FAIL / 3 SKIP, 1,932 total; all eleven H14 cases pass together. Build, typecheck, lint and diff PASS. Historical H14 remains FAIL: 1,918 PASS / 11 FAIL / 3 SKIP; its directed repairs did not themselves establish global PASS. Physical/package/release gates remain separate. |
| YF-34 | Unsigned package, license/privacy and release gates | OPEN RELEASE BLOCKER. No signing, license/privacy review or final package acceptance is claimed here. |
| YF-35 | CPU contention and stutter under real workloads | PARTIAL. A01 adds bounded diagnostics and synthetic measurements; concurrent game/OBS/GPU behavior is unmeasured. |
| YF-36 | Removing YouTube channel settings can reset search configuration | TECHNICAL PASS. B01 preserves unrelated search configuration when channel settings are removed. |
| YF-37 | OBS browser source for avatar visuals | PARTIAL. F02 implements an opt-in loopback pixel stream with an ephemeral 256-bit capability and directed HTTP tests. Hidden-window rendering, lip-sync and OBS/Windows resource impact still require physical acceptance with a disposable test profile and fixture model. |
| YF-38 | User-controlled Windows start-at-login | PARTIAL. F01 implements an opt-in Windows startup setting with background launch and tray behavior; directed tests pass. Real Windows startup, disable, tray recovery and microphone state remain unaccepted. |
| YF-39 | Configurable wake phrase | FUTURE / DEFERRED by explicit product decision: preserve the remaining 33% weekly Astra allowance for current priorities. No wake-word detection, background microphone activation, or new dependency is authorized. It is not a blocker for the current scoped release. G01's prior research remains evidence only: no deployable licensed Spanish model with validated offline/resource/false-trigger behavior was established. |
| YF-40 | Hands-free end-of-turn after wake phrase | PARTIAL / DIRECTED CORRECTION. H14 retains a VAD stop received during asynchronous capture startup and resumes the existing remaining silence grace. Exactly-once/manual/cancel regressions pass; H13 physical auto-submit failure remains open. Wake activation stays deferred. |
| YF-41 | Cancel microphone input before submission | PARTIAL / DIRECTED TECHNICAL PASS. H14 preserves pre-commit cancel, barge-in, stale callback fences and transport retirement. A missing bridge finalization wakeup was corrected without extending timeout. Physical H13 success is not established. |

## Corrección del estado físico más reciente (H19)

El último candidato instalado demostró **chat escrito PASS**, **micrófono sin envío de turno FAIL**, **inicio de respuesta hablada excesivamente lento FAIL** y **silbido agudo TTS conocido y sin resolver**. OBS, RVC y cambio real de dispositivos no fueron aceptados completamente. Estos resultados prevalecen sobre cualquier estado técnico antiguo incompatible.

**YF-28:** BLOCKED / UNVERIFIED / NOT IMPLEMENTED.

**YF-39:** FUTURE / DEFERRED.

Ver [estado y límites de distribución](YUKI_H19_PUBLIC_STATUS.md).
