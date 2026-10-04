# Aside Free LLM Autopilot

**English** | [한국어](README.ko.md)

## Put free LLMs to work in Aside.

**Find free models. Connect them. Let your agent keep the setup current.**

An Aside-first skill that guides your agent through provider discovery, authorized signup, model setup, browser-task verification, and daily maintenance. Start with offers such as OpenCode Zen / Space Bunny, OpenRouter, and NVIDIA, then adapt to what actually works in your environment.

[Get started](#get-started) · [How it works](#how-it-works) · [Provider starting points](#provider-starting-points) · [Project status](#project-status) · [Read the skill](SKILL.md)

> “Free” means **zero incremental LLM API spending on eligible routes**. It does not mean free Aside access, a free setup model, or unlimited usage. Independent community project; not affiliated with Aside or the model providers.

## A free model list is only the beginning

Finding a free offer is easy. Getting it to finish a browser task is harder.

An API may answer a short prompt but reject an agent's larger context. A trial may expire. A model may support chat but not the tools Aside needs. Keeping track of accounts, settings, and changing limits becomes another task.

The goal here is simple: **get a free model working in your Aside, then keep your managed routes useful.**

| What you want | What the skill guides your agent to do |
| --- | --- |
| Less setup work | Inspect your environment, reuse accounts, and connect eligible providers |
| A usable model | Verify a real public browser task, not just a successful API response |
| Current free options | Discover new offers and recheck existing ones daily |
| Clean configuration | Remove retired managed routes while preserving temporary failures for retry |
| A portable setup | Follow the installed app's current tools and settings instead of hardcoded paths |

## How it works

```text
Inspect your environment and existing accounts
                    ↓
Discover free offers → complete eligible signup
                    ↓
Connect to Aside → read a public page → verify the final answer
                    ↓
Daily maintenance
    ├─ Add newly verified routes
    ├─ Cool down temporary failures
    ├─ Remove expired or paid routes
    └─ Update local provider knowledge
```

The agent uses the browser, authentication tools, model settings, and scheduler you already have. No bundled server, custom daemon, container, or routing script is required.

## Get started

### What you need

- A working [Aside](https://aside.com/) installation and a model that can perform the initial setup.
- Your designated signup account and access to its normal verification flow.
- Permission to save a user skill and update the relevant model configuration.
- A supported routine scheduler for daily maintenance, with a host and executor available when it runs.

You do not need to paste passwords, API keys, or verification codes into chat. The agent should use the available credential tools and local secret storage.

### 1. Paste this into Aside

```text
Read https://github.com/sojuhub/aside-free-llm-autopilot/blob/main/SKILL.md
and install Aside Free LLM Autopilot for my current Aside environment.

First inspect my profile, existing accounts, model settings, and routines.
For eligible new free providers, use my designated personal account to
accept ordinary free-account terms, sign up, verify access, and connect API keys.
If the signup identity is not established, ask me for it.
Do not print keys or verification codes. No payments, cards, or auto-recharge.

Verify one public browser task with a free model, including the final answer.
Keep my current defaults and explain how to select the verified free model.
Register one daily maintenance routine at 09:00 in my local timezone,
reusing an existing matching routine.
Add newly verified routes, remove retired or paid managed routes,
and update provider knowledge in the installed SKILL.md.
Report actual successes separately from blocked or unverified steps.
```

The agent should discover the correct user-skill location for your installation. To install manually, download [SKILL.md](SKILL.md) and place it at `<your user-skill directory>/aside-free-llm-autopilot/SKILL.md`. Confirm that your agent discovers it, then run the setup request above. Installing the file alone does not activate account onboarding or a routine.

Already installed as `free-llm-autopilot`? Ask the agent to migrate that installation's name and references to `aside-free-llm-autopilot`, preserving its configuration, accounts, and existing routine. Do not install a second maintenance owner.

### 2. Check your first success

Look for concrete results:

- The exact provider and model selectable in Aside.
- A browser-tool result and a final answer grounded in a public page.
- Evidence for free eligibility, with remaining limits identified.
- The routine's enabled state, timezone, and next scheduled run.

If a step fails, continue that step. Account creation, model import, and browser-task completion are separate milestones.

### 3. Use it in everyday work

**Research a public page**

```text
Use Aside Free LLM Autopilot to choose an eligible free model
and summarize this public page. If no free route is available, tell me.
```

**Refresh the setup**

```text
Check my free LLM connections and discover new eligible offers.
Cool down temporary quota errors and remove only confirmed retired routes.
```

**Choose a free default**

```text
Set a verified free model as the default for new general Aside tasks.
Tell me which categories changed and preserve my important-work settings.
```

You can also select a model directly. This skill teaches agent-directed setup and selection; it does not intercept every GUI request or migrate tasks already in progress.

## Provider starting points

These are discovery leads, **not a guarantee that every provider works in Aside**. Documentation baseline: October 4, 2026. Recheck on setup.

| Provider | What to verify | Official source |
| --- | --- | --- |
| OpenCode Zen / Space Bunny | Limited-time free offers; exact model pricing, allowed clients, and data policy | [Zen](https://opencode.ai/docs/en/zen/) |
| OpenRouter Free | Required capabilities, current free limits, and actual selected model; selection is not a quality ranking | [Free Router](https://openrouter.ai/openrouter/free) |
| NVIDIA API Catalog | Trial conditions, account eligibility, quota, and permitted data/use | [Quickstart](https://docs.api.nvidia.com/nim/re/docs/api-quickstart) |
| Gemini | Current free-tier model, region, account billing, and data treatment | [Pricing](https://ai.google.dev/gemini-api/docs/pricing) |
| Groq | Whether the complete Aside prompt fits the available token/request limits | [Rate limits](https://console.groq.com/docs/rate-limits) |
| Cerebras | Current free offer and actual client compatibility | [Documentation](https://inference-docs.cerebras.ai/) |

Space Bunny is documented by Zen as a limited-time free offer with a provider no-retention/no-training policy. Other free models have different conditions. A “Free” label is not permission to send sensitive account or customer data.

## What daily maintenance does

| Change detected | Intended action |
| --- | --- |
| New eligible provider or model | Check conditions → authorized signup → connect and verify → add |
| Paid conversion or expired free offer | Remove the owned route from active selection |
| 429 or temporary outage | Keep the entry and wait until an appropriate retry time |
| Expired authentication | Restore access where supported or report the required user step |
| Official catalog unavailable | Preserve settings and avoid newly selecting an unverified route |

Only routes added by this skill or explicitly assigned to it are managed. Unrelated settings, accounts, and shared keys stay intact. The default daily discovery budget is at most three new providers and 15 minutes, so maintenance does not consume the entire free allowance.

Your host, tools, and execution model must be available for a routine to run. A saved schedule is not proof of a completed daily check. Updating your local SKILL.md also does not publish changes to this repository automatically.

## Small package, clear responsibilities

| File | Purpose |
| --- | --- |
| [README.md](README.md) | Complete English introduction, setup, usage, and troubleshooting |
| [README.ko.md](README.ko.md) | Complete Korean guide |
| [SKILL.md](SKILL.md) | Self-contained instructions the agent executes |
| [LICENSE](LICENSE) | MIT license |

The skill adapts to current Aside capabilities rather than requiring one person's profile, paths, or model names. Other agent environments can follow it when they have the necessary tools, but Aside is the primary target.

## Project status

**Experimental, instruction-based skill. Ready to install and evaluate.**

- **Current skill:** passed Codex and Aside format validation. Includes profile discovery, configuration readback, actual-response checks, and routine verification.
- **Prior personal setup:** Space Bunny and OpenRouter completed Aside tool calls. These historical observations are not a fresh-install result for this public package.
- **Observed limitations:** an NVIDIA multi-step task hit quota; a Groq task exceeded an initial-input limit. Installation rechecks current behavior rather than treating these as permanent failures.
- **Not yet established:** end-to-end onboarding across diverse user environments, universal new-provider signup success, and sustained unattended daily operation.

We separate a listed model from a verified route. Availability, authentication, and model quality can leave individual steps incomplete.

## FAQ

**Is Aside itself free?**  
This project does not change Aside's pricing. It targets eligible LLM API spending. The model running initial setup or daily maintenance has its own access and cost conditions.

**Will it run as soon as I install the file?**  
No. Run the setup request to connect accounts, verify a route, and register a routine. Markdown is an instruction source; the agent and scheduler perform the work.

**Will it sign up for every service it finds?**  
It onboards eligible providers within your designated account and authorization. Payment requirements, incompatible conditions, and unsupported verification steps are reported. Existing accounts are checked first.

**What happens when all free options are unavailable?**  
Free-only operation stops and reports the problem. It does not silently buy credits or use paid APIs. Existing-subscription fallback requires your chosen policy.

**Can I use it for private work?**  
Only with a route whose current data policy and quality meet your requirements. Free discovery and probes use public content. Cheap availability alone does not justify moving sensitive work.

## Troubleshooting and rollback

| Symptom | Next check |
| --- | --- |
| Skill not found | Verify the actual user-skill directory and whether this session loaded it |
| Model listed but task fails | Inspect actual response model, tools, prompt size, and quota |
| Signup interrupted | Continue the unfinished step in the existing browser session |
| Daily run missing | Check enabled state, timezone, next run, host, authentication, and last execution receipt |
| Want to stop | Pause the matching routine first, then restore only this skill's settings from the saved prior values |

For removal, ask the agent to remove managed model entries and the installed skill. Shared credentials and accounts are preserved; account closure or key revocation is a separate request.

## Contribute

[Open an issue](https://github.com/sojuhub/aside-free-llm-autopilot/issues) with your Aside version, OS, provider/model, failing step, and a sanitized error. Do not include account emails, API keys, verification codes, or private browser screenshots.

For a provider suggestion, include an official pricing/conditions link and the date checked. Distinguish a basic API response, a successful Aside tool call, and a complete browser task. Keep both README versions aligned when changing user-facing behavior.

## License

[MIT](LICENSE). The full license is also embedded in [SKILL.md](SKILL.md#license) so the skill can be distributed on its own.
