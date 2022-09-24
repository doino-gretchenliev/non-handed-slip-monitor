# Non-handed slip monitor (Bulgaria)

This automation uses GitHub Actions to check periodically(every hour) for non-handed slips.

## Requirements

 - GitHub account
 - Enabled notifications for GitHub Actions

![Enabled notifications for GitHub Actions](https://github.com/doino-gretchenliev/non-handed-slip-monitor/blob/main/1.png?raw=true)


## How to use

1. Fork this repository
2. Set two secrets for your new repository:
   - `DRIVING_LICENCE_NUMBER`: your driving license number
   - `OBLIGED_PERSON_IDENT`: your personal identifications number(ЕГН)
![GitHub Actions Secrets](https://github.com/doino-gretchenliev/non-handed-slip-monitor/blob/main/2.png?raw=true)
3. Done.

## Privacy concerns

1. The only executable code(GitHub Action workflow) is located [here](https://github.com/doino-gretchenliev/non-handed-slip-monitor/blob/main/.github/workflows/main.yml).
2. It utilizes only open source technology - Ubuntu, CURL, and JQ.
3. Secrets are stored in [encrypted form by GitHub](https://docs.github.com/en/actions/security-guides/encrypted-secrets).
4. You can configure your repository as private.