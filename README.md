<<<<<<< HEAD
# utrata
proste utrata
=======
# Útrata – instalace

Data se ukládají jen lokálně v prohlížeči zařízení (localStorage). Aplikace nedělá žádné síťové požadavky s daty.

## 1. Nasazení (jednorázově) – GitHub Pages
1. Nový **veřejný** repozitář (Pages na privátním repu vyžaduje placený GitHub plán), nahraj všech 5 souborů do rootu.
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, `/ (root)`.
3. Za chvíli běží na `https://<user>.github.io/<repo>/`.

Kód je veřejný, data ne – zůstávají v zařízení.

## 2. iPhone
Safari → otevři URL → Sdílet → **Přidat na plochu**. Pak spouštěj vždy z ikony na ploše (běží offline a iOS data aplikace na ploše nemaže; u obyčejného webu v Safari je může po 7 dnech nepoužívání smazat).

## 3. Mac
Safari → otevři URL → menu **Soubor → Přidat do Docku** (macOS Sonoma a novější).

## Přenos dat Mac ↔ iPhone
Nastavení → **Export JSON** na jednom zařízení → AirDrop → **Import JSON** na druhém. Import přepíše data cílového zařízení.
Export dělej i jako zálohu.

## Logika limitu
- Každý den: `zůstatek += denní limit − útrata`.
- Dnes můžeš utratit = `limit + převod z minulých dní − dnešní útrata`.
- Změna limitu platí od dneška, historie se nepřepočítává.

## Update aplikace
Nahraj nové soubory do repa. Service worker je network-first → při dalším spuštění online se načte nová verze.
>>>>>>> ae170f3 (initial commit)
