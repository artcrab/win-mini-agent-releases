# win-mini-agent Terms of Use

**The Korean version prevails.**

> **Summary - The full terms below prevail**
> 1. The Program is free. The User is responsible for any fees charged by the Model Provider.
> 2. The content the User enters and the file contents the agent reads during a task and sends to the model are sent to the Model Provider.
> 3. In the default full-access mode, the agent can delete files with the User’s Windows permissions and run commands without a separate click.
> 4. Update installation starts only when the User clicks to install it. To reduce the risk of loss, backing up important files in advance and monitoring the agent is recommended.
> 5. The User may stop using the Program at any time. Warranties and liability are governed by Articles 16 and 17, and liability that the law does not allow to be excluded or limited is not limited.

## Article 1. Purpose

These Terms govern the use of win-mini-agent, a Windows program distributed free of charge by the Author (GitHub account artcrab).

## Article 2. Definitions

1. **Author** means the Author (GitHub account artcrab).
2. **User** means a person who uses the Program under these Terms.
3. **Program** means the two Windows executable files in the win-mini-agent release, `win-mini-agent.exe` (API edition) and `win-mini-agent-codex.exe` (Codex edition).
4. **Release Repository** means the `artcrab/win-mini-agent-releases` repository on GitHub.
5. **Model Provider** means the entity providing the AI model service used by the Program’s agent.
6. **Working Folder** means the folder the User designates for the agent’s work.
7. **Output** means materials, including responses and files, that the agent generates or modifies at the User’s request.

## Article 3. Publication, Effect, and Acceptance

These Terms are posted in the Release Repository as `약관.md`. The README and release notes link to this file, and a copy of the Terms is attached to each release. The User may read and download a copy of the Terms from the Release Repository at any time.

**By using the Program after these Terms have been made available for review, the User is deemed to accept them.** Any ambiguity in the Terms is interpreted in the User’s favor.

If the Author and the User separately agree on terms different from these Terms, that agreement prevails over these Terms. Matters not covered by these Terms are governed by the relevant laws.

A minor uses the Program with the consent of their legal guardian.

## Article 4. License and Restrictions

The Author grants the User a **free, non-exclusive, non-transferable** license to download, install, and run the Program for their own use on Windows PCs they use. This license is granted per individual User. This free license includes the User’s own use at work when the User’s employer allows it. Installation for multiple people by an organization on shared PCs or through central deployment, and operation of the Program as an internal service by an organization, are not covered by this free license.

Operating the Program to provide its functions to third parties, or processing third parties’ requests as a service, is not covered by this license. The same applies to offering the Program as part of a paid installation or support product or as part of another product or service.

A person who receives the executable file from someone else does not receive a license through that transfer. That person receives the license from the official release page in the Release Repository, under the Terms posted there.

- Except as permitted by law, the User may copy the Program only as needed for their own use on PCs they use.
- Except as permitted by law, the User may not redistribute the Program.
- Except as permitted by law, the User may not resell or rent out the Program.
- Except as permitted by law, the User may not modify the Program.
- Except as permitted by law, the User may not reverse engineer the Program.

The User may make preservation copies, make copies to investigate, research, or test functionality, and reverse engineer program code as needed for interoperability, as permitted by the Copyright Act. Information obtained by reverse engineering program code may be used to the extent permitted by law. Editing the configuration and instruction files the Program provides (`config.toml`, `user.md`, `soul.md`, `prompts`, `skills`) is not a modification of the Program.

## Article 5. Ownership of Rights

Copyright and other intellectual property rights in the Program belong to the Author or the applicable rights holders. The User receives the license in Article 4. The User retains any rights they already hold in materials they provide. Use of Output is also subject to the Model Provider’s terms and the rights of third parties.

## Article 6. Open-Source Components

Third-party open-source components included in the Program are governed by their respective licenses. The licenses and notices are available in `THIRD_PARTY_NOTICES.txt` and `THIRD_PARTY_SKILLS.md`, which come with the release. These Terms do not restrict the rights those licenses grant to the User.

## Article 7. Third-Party Services

When the User uses a Model Provider’s service, Codex or ChatGPT, or GitHub in connection with the Program, each service’s terms, fees, and data handling policies apply.

**The content the User enters in the Program and the file contents the agent reads during a task and sends to the model are sent to the Model Provider. The Author does not receive this content.** Article 10 describes the information sent.

## Article 8. User Obligations and Prohibited Conduct

The User must comply with applicable laws. Before using materials from a workplace or other organization to which the User belongs, the User must check and follow that organization’s rules.

The User must not use the Program for unlawful purposes, attack systems belonging to others, or generate or use content that infringes the rights of others.

## Article 9. AI Output

**AI Output may be incorrect. Before using it, the User must check its accuracy and suitability for the intended purpose.**

AI Output is not professional legal, tax, medical, or financial advice. The agent operates with the User’s Windows permissions. When the agent changes files or runs commands, those actions are already carried out before the User checks the result.

## Article 10. Data and Personal Information

**The Author collects no User information or personal information through the Program and maintains no personal information files.** This statement concerns what the Program does. The Program has no separate feature that transmits usage data. What the Author can see on GitHub is GitHub’s aggregate statistics, such as download counts per release file and repository visit counts; the Program does not send the Author the identity or IP address of the people who download.

When checking for updates, the Program requests the latest release information, `release.json` and `release.json.minisig` from the GitHub API, and when the User clicks install, it receives the new executable file in the same way. Files may be delivered from GitHub's file storage (githubusercontent.com). GitHub can see the request’s IP address and the User-Agent value `win-mini-agent-updater`. Only if a token is stored, the Program sends it in the authorization header to the API address set in `[update] api_base` of `config.toml` (default `https://api.github.com`). The token is not sent to the file storage (githubusercontent.com). Anyone can see the download count for each release file on GitHub. GitHub’s data handling policy applies to this information.

The API edition obtains the API key from the `OPENAI_API_KEY` environment variable or the `win-mini-agent/api-key` entry in Windows Credential Manager to authenticate model requests. The default model endpoint is `https://api.openai.com/v1`. The model endpoint can be changed in `config.toml` to another address, such as a company Azure endpoint. In that case the request contents and the API key are sent to the address the User set. If the User sets an `http://` address instead of `https://`, the request contents and the API key may be sent unencrypted. **The API edition sends the Model Provider the content the User enters and any file contents the agent reads during a task and includes in a model request.** The Model Provider’s data handling policy applies to the information sent.

The Codex edition (`win-mini-agent-codex.exe`) runs the official Codex CLI that the User installed and signed in to with `codex login`. What the Program passes to the Codex CLI is the task the User enters, the role instructions (`soul.md`, `user.md`, `prompts` and skills) and the Working Folder path. **The Codex CLI runs under the User’s ChatGPT/Codex account and can itself read files and run commands during a task and send their contents to OpenAI.** What the Codex CLI reads, sends, and stores is governed by the terms and policies that apply to the Codex CLI and the User’s OpenAI account. The Program does not read or store those sign-in credentials. The Codex edition is used only with the User’s own account on a PC the User uses.

The contents of `soul.md`, `user.md`, and `prompts` are included in every model request. Requests for the planning role also include the skill list (names and descriptions); requests for the working and reviewing roles also include the bodies of the selected skills.

In full-access mode, commands the agent runs can themselves connect to the internet or send data, separately from model requests. Such transmissions are different from the model requests described above, and the policies of the places those commands connect to apply.

By default, the Program folder’s `config.toml`, `user.md`, `soul.md`, `prompts`, `skills`, `data`, and `logs`, as well as the Working Folder, are stored on the User’s PC. Task records (what the User entered, the model’s replies, and tool results) are kept in the `data` folder and the Program’s operation log in the `logs` folder; the User can delete them by deleting those files. If the agent reads a stored file and includes its contents in a model request, those contents are sent to the Model Provider. The Program interface is served only on `127.0.0.1` (this PC).

## Article 11. Full-Access Mode and Backups

**Full-access mode is the default. In this mode, the agent can read, change, overwrite, or delete any file the User’s Windows account can access, including files outside the Working Folder. It can run commands without a separate click from the User.**

Setting `restricted_mode = true` in the `[security]` section of `config.toml` turns on restricted mode, which works differently in each edition. In the API edition’s restricted mode, file work is limited to the Working Folder, commands can run only if turned on in `[shell]`, and running a command or overwriting an existing file requires a click from the User. In the Codex edition’s restricted mode, the Codex CLI for the working role runs in the `workspace-write` sandbox; the planning role runs in the `read-only` sandbox in either mode, and the reviewing role does so by default. **In every edition and mode, file contents the agent reads and passes to the model are sent to the Model Provider.**

To reduce the risk of loss, it is advisable to back up important files in advance, monitor the agent’s work, and stop it if it takes an unintended action. In full-access mode, commands run without step-by-step approval, so monitoring alone cannot stop every action before it runs.

## Article 12. Updates

By default, the Program automatically checks for a new version at startup. It also checks when the User clicks the on-screen button to check for updates. **Update installation starts only when the User clicks to install it.** On install, the Program receives the new executable file from the GitHub API, and the file may be delivered from GitHub's file storage (githubusercontent.com). When checking for updates, the Program verifies the signature of `release.json`; when installing, it compares the SHA-256 hash of the downloaded executable with `release.json`. The Program does not check files the User downloads directly from the Release Repository; the User can compare such a file’s SHA-256 hash with the value in `release.json`.

To turn off the startup update check, set `check_at_start = false` in the `[update]` section of `config.toml`. If `repo = ""` is set in the same section, the Program makes no connections for updates.

## Article 13. Changes to the Terms and Notice

When the Author changes these Terms, the Author gives notice by posting the new Terms and their effective date in the Release Repository.

**A copy the User has already received remains subject to the Terms in effect when the User received it. The new Terms apply to copies newly downloaded or updates installed by the User on or after the effective date.** If the User rolls back to, or downloads again and uses, an earlier version, the Terms attached to that version’s release apply.

## Article 14. Free Distribution and Fees

**The Program is provided free of charge. The Author does not sell the Program for payment or accept payment for its use.** If the model service incurs fees, the service’s fee terms apply between the User and the Model Provider.

## Article 15. Duration and Termination

**The User may end their use at any time by stopping use of the Program. If the User breaches these Terms, the license granted under these Terms ends due to that breach.** When the license ends, the User must stop using the Program.

## Article 16. Disclaimer of Warranties

**To the extent permitted by law, the Program is provided as is in its current state. The Author does not warrant that the Program is suitable for the User’s purpose or will operate without errors.**

Whether some Program behavior on Windows has been verified is unconfirmed. Whether the stop button works on Windows is unconfirmed. **In full-access mode, the agent can overwrite or delete files and run commands with the User’s Windows permissions. This can result in lost files or actions the User did not intend.**

## Article 17. Limitation of Liability

**Liability arising from the Author’s intentional conduct or gross negligence is neither excluded nor limited.**

The Program is provided free of charge, and the Author receives no payment for its use. For these reasons, **to the extent permitted by law, compensation for damage caused by the Author’s ordinary negligence is limited to ordinary damages.**

**The warranty disclaimer and liability limitations in these Terms do not apply to liability that the law prohibits excluding or limiting, including liability under the Product Liability Act.**

## Article 18. Export and Import Laws

When using the Program, which uses cryptographic signature verification (minisign/Ed25519), SHA-256 hash verification, and TLS, the User must comply with the export and import laws applicable where the Program is used.

## Article 19. Severability

If any provision of these Terms is invalid, the remaining provisions remain in effect. The entire agreement is invalid if its purpose cannot be achieved through the valid provisions alone or if keeping only those provisions would be unfairly disadvantageous to either party.

## Article 20. Language

**The Korean version prevails.** If the Korean Terms and the English translation differ, the Korean Terms apply.

## Article 21. Governing Law and Jurisdiction

The laws of the Republic of Korea govern these Terms and use of the Program.

The court with jurisdiction over a dispute is determined under the Civil Procedure Act.

## Article 22. Effective Date and Version

These Terms take effect on 2026-11-20. This is version 1.0.
