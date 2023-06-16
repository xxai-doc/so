<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Waxaa lagu talinayaa in la rakibo nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) marka hore, ka dibna `direnv allow` ka dib gelitaanka tusaha ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) si toos ah ayaa loo fulin doonaa ka dib marka la galo tusaha).

Macnuhu waa: Turjumaadda Shiinaha ee Jabbaan, Kuuriyaan, Ingiriisi, Ingiriisi oo loo turjumay dhammaan luqadaha kale. Haddii aad rabto inaad taageerto Shiinaha iyo Ingiriisiga, waxaad qori kartaa `zh: en` .

Macnuhu waa: Turjumaadda Shiinaha ee Jabbaan, Kuuriyaan, Ingiriisi, Ingiriisi oo loo turjumay dhammaan luqadaha kale. Haddii aad rabto inaad taageerto Shiinaha iyo Ingiriisiga, waxaad qori kartaa `zh: en` .

* [code-dhamaadka hore](https://github.com/xxai-art/web)
* [Xirmooyinka luqadda ee goobta guud ahaan](https://github.com/xxai-art/web/tree/main/i18n)
* [Xirmooyinka luqadda ee cutubyada gelitaanka](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Shabakadda Dukumentiyada Luuqadaha Badan](https://github.com/xxai-doc)

Luuqadda hore ee barnaamijka afku waa [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , kaas oo ku daraya qaar ka mid ah sifooyin ku salaysan qoraalka kafeega, eeg [./coffee_plus.md](./coffee_plus.md) .

## Caalamiga ah ee mareegaha iyo dukumentiyada

Ku dhis 3 mashruuc ee soo socda

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Dabagalku waa `.mdt` , waxaad isticmaali kartaa syntax la mid ah `<+ ./coffee_plus/import.js>` si aad u tixraacdo faylalka dibadda, oo aad dhaliso calaamadayn leh daba-gal `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Turjumaada calaamadaynta ma tarjumi doonto summada iyo isku xidhka, waxayna kaydin doontaa weedhaha la turjumay. Haddii tarjumaadda wax laga beddelo laakiin qoraalka asalka ah aan la beddelin, fulinta mar kale dib uma qori doonto beddelka tarjumaada.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Faylasha luqadda ee tarjumaadda mareegaha `yaml` ee la sameeyay

### Dukumentiga Turjumaada Tilmaamaha Automation

Eeg kaydka koodka [xxai-art/doc](https://github.com/xxai-art/doc)

Waxaa lagu talinayaa in la rakibo nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) marka hore, ka dibna `direnv allow` ka dib gelitaanka tusaha ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) si toos ah ayaa loo fulin doonaa ka dib marka la galo tusaha).

Si aan uga fogaado saldhigga weyn ee koodka ee loo turjumay boqollaal luqadood, waxaan sameeyay saldhig kood u gaar ah luqad kasta waxaanan abuuray urur kaydiya saldhigga koodka.

Dejinta doorsoomiyaha deegaanka `GITHUB_ACCESS_TOKEN` ka bacdi ku socodsiinta [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) ayaa si toos ah u abuuri doonta kaydka koodka.

Dabcan, waxaad sidoo kale ku dhejin kartaa saldhigga koodhka.

Tixraaca qoraalka tarjumaada [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Koodhka qoraalka waxa loo fasiray sidan soo socota:

[bunx](https://bun.sh/docs/cli/bunx) waa bedelka npx, kaas oo dhakhso badan. Dabcan, haddii aadan ku rakibin bun, waxaad isticmaali kartaa `npx` beddelkeeda.

`bunx mdt zh` wuxuu ka dhigayaa `.mdt` tusaha zh sida `.md` , eeg 2 faylasha ku xidhan hoos

* [kafee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kafee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` waa furaha koodka tarjumaadda (haddii aad kaliya ku rakibtay `nodejs` , laakiin `bun` iyo `direnv` aan la rakibin, waxaad sidoo kale ordi kartaa `npx i18n` si aad u turjunto).

Waxay kala saari doontaa [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , qaabaynta `i18n.yml` ee dukumeentigan waa sida soo socota:

```
en:
zh: ja ko en
```

Macnuhu waa: Turjumaadda Shiinaha ee Jabbaan, Kuuriyaan, Ingiriisi, Ingiriisi oo loo turjumay dhammaan luqadaha kale. Haddii aad rabto inaad taageerto Shiinaha iyo Ingiriisiga, waxaad qori kartaa `zh: en` .

Kan u dambeeya waa [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , kaas oo soo saara nuxurka u dhexeeya cinwaanka ugu weyn iyo cinwaanka hoosaadka ugu horreeya ee luqad kasta `README.md` si loo soo saaro `README.md` . Koodhku aad buu u fudud yahay, adiguba waad eegi kartaa.

Google API waxa loo isticmaalaa tarjumaad bilaash ah. Haddii aadan geli karin Google, fadlan hagaaji oo deji wakiil, sida:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Qoraalka tarjumaadda ayaa soo saari doona kayd la turjumay `.i18n` directory, fadlan ku hubi `git status` oo ku dar kaydka koodka si aad uga fogaato turjumaada soo noqnoqda.

Fadlan socodsii `bunx i18n` mar kasta oo aad wax ka beddesho tarjumaada si aad u cusboonaysiiso kaydka.

Haddii qoraalka asalka ah iyo tarjumaada isku mar la beddelo, khasnadku wuu wareeri doonaa, markaa haddii aad rabto inaad wax ka beddesho, waxaad kaliya beddeli kartaa mid, ka dibna ku socodsii `bunx i18n` si aad u cusboonaysiiso kaydka.
