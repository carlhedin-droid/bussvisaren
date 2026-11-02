# Bussvisaren

Avgångstavla för bussarna mellan Sandudden/Träkvista (Ekerö) och Brommaplan.

- **Till Brommaplan:** Sanduddens vägskäl och Träkvista. Bussar med slutstation Brommaplan (309, 311) samt 176/177 mot Mörby station, som går via Brommaplan.
- **Hem:** från Brommaplan med 309, 311 och 177, plus reservlinjerna 176 (Ekvägen) och 302 (Träkvista idrottsplats). Markeringarna "Hinner gå / Spring / Hinner inte" utgår från att man står vid tunnelbanedörren när tåget rullar in på Brommaplan: springa till bussen tar ca 2 min, gå ca 4 min.

- **Skjuts:** på fliken Hem trycker man på en avgång och sedan på "Jag vill ha skjuts". Då skickas en push-notis via Homey (flödet "🚌 Skjuts från Brommaplan", webhook-händelserna `skjuts_till_sara` och `skjuts_till_calle`) med linje, avgångstid och upphämtningstid vid Träkvista (309, 311, 177), Ekvägen (176) eller Träkvista idrottsplats (302). Upphämtningstiden är SL:s realtid för samma tur vid den hållplatsen; finns den inte uppskattas 13 min. Vem man är väljs en gång och sparas i telefonen.

Data i realtid från SL:s öppna API (SL Transport, via Trafiklab). Ingen nyckel krävs.
Publiceras med GitHub Pages från grenen `main`.
