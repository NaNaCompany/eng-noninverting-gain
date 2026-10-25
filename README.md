# 비반전 연산증폭기 이득 계산기

이상 연산증폭기의 비반전 음귀환 전압이득 계산

- Plan ID: E086
- App: https://nanalab.kr/eng-noninverting-gain/
- Repository: https://github.com/NaNaCompany/eng-noninverting-gain
- Formula: `A_v = 1+R_f/R_g`
- Output: 비반전 전압 이득 A_v

## Model

R_f≥0, R_g>0. 음귀환이 유지되는 선형 이상 연산증폭기 모델이다. 전원 레일 포화·대역폭·입력 오프셋·출력 부하는 제외한다.

Inputs are normalized to SI. Only one scalar is returned. Model conditions, finite numbers, physical boundaries, overflow and underflow are checked. External solver APIs and property databases are not used.

## Verification

Run `node --test tests/*.test.mjs` with Node.js 22 or later. Independent 70-digit Decimal example result: `10`. Source and license notices are in [SOURCES.md](SOURCES.md) and [LICENSE](LICENSE).

## Hosting

GitHub Pages uses `main` and `/`, with the NaNaCompany domain inherited. Google GTM, GA4, AdSense, Cloudflare analytics and the gray More Apps link are included. All code, descriptions and graphics are original.

## Static languages

Korean (existing root), English (`en/`), Spanish (`es/`), Simplified Chinese (`zh/`), Japanese (`ja/`) and German (`de/`). Each page has its own canonical URL, reciprocal hreflang, localized metadata, interface, validation messages and preview image. The language links work without JavaScript. Calculation code is shared and no runtime translation API is used.

Edit `localization/*.json` for text, `src/template.html` for the shared page, and run `python scripts/build-locales.py`. Run `python scripts/build-locales.py --check` and `npm test` before publishing. Decimal commas are accepted in Spanish and German; thousands separators are not supported.
