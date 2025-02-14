<script>
  import t1 from "$lib/images/t1.jpeg";
</script>

<svelte:head>
  <title>Biografija</title>
  <meta name="description" content="Biografija Lexington benda" />
</svelte:head>

<section class="bio-section">
  <img class="mob" src={t1} alt="Lexington background" />
  <img class="desk" src={t1} alt="Lexington background" />
  <div class="bio-text">
    <h1>Lexington band</h1>

    <p>
      Lexington Band je pop rock sastav iz Srbije, osnovan 2004. godine u
      Beogradu. Osnivači benda su Bojan Vasković (vokal), Miloš Vuksanović (bas
      gitara), Dragoljub Stević (gitara), Dejan Krstić (bubnjevi) i Đorđe
      Erčević (klavijature). Od svog osnivanja, bend je postao jedan od
      najpoznatijih i najomiljenijih sastava na muzičkoj sceni Balkana.
    </p>

    <h2>Početak Karijere</h2>
    <p>
      Lexington Band je počeo svirajući na lokalnim svirkama i malim klubovima u
      Beogradu, gde su brzo stekli popularnost svojim energičnim nastupima i
      emotivnim pesmama. Njihova muzika se prepoznaje po melodičnim aranžmanima
      i tekstovima koji govore o ljubavi, gubicima i životnim izazovima.
    </p>

    <h2>Diskografija</h2>
    <p>
      Prvi veći uspeh doživeli su sa singlom <span class="italic"
        >“Kako je tako je”</span
      >, koji je postao hit i stekao veliku popularnost. Nakon toga su usledili
      mnogi hitovi koji su obeležili njihovu karijeru.
    </p>

    <h3>Albumi:</h3>
    <ul>
      <li>
        <span class="italic">“Kako je tako je”</span> (2010) - Debi album koji je
        sadržao hitove kao što su “Ja sam tvoj i kad nema ko” i “Da me malo hoće”.
        Ovaj album je cementirao njihovo mesto na muzičkoj sceni i postao jedan od
        najprodavanijih albuma te godine.
      </li>
      <li>
        <span class="italic">“Ma sretno 2012”</span> (2012) - Album koji je doneo
        još veći broj hitova, uključujući pesme “Dobro da nije veće zlo” i “Pijane
        usne”, “Miris karmina”, “Bol je uvek ista”.
      </li>
      <li>
        <span class="italic">“Balkanska pravila”</span> (2014) - Ovaj album je obeležio
        promenu u zvuku benda, sa više eksperimentalnim i kompleksnim aranžmanima.
        Pesme koje su ostavile trag i postale veliki hitovi: “Dođi ove noći”, “Potraži
        me”.
      </li>
      <li>
        <span class="italic">“Noć pod zvijezdama”</span> (2017) - Uz ovaj album je
        išao Live album snimljen tokom koncerta na Tašmajdanu, koji prikazuje njihovu
        energiju i snagu nastupa uživo.
      </li>
      <li><span class="italic">“Lavovu”</span> (2024)</li>
    </ul>

    <h2>Koncerti i Festivali</h2>
    <p>
      Lexington Band je poznat po svojim dinamičnim i energičnim nastupima
      uživo.
    </p>
    <p>
      Nastupali su na brojnim festivalima i koncertima širom Balkana,
      uključujući:
    </p>
    <ul>
      <li>EXIT Festival (Novi Sad)</li>
      <li>Beogradska Arena, Belgrade Beer Fest (Beograd)</li>
      <li>Skopje Fest (Skoplje)</li>
      <li>Ulaz Festival (Beograd)</li>
    </ul>
    <p>
      Jedan od najznačajnijih trenutaka u njihovoj karijeri bio je koncert na
      beogradskom Tašmajdanu 2017. godine, gde su okupili više od 10,000 fanova,
      ovaj koncert je zabeležen na njihovom live albumu “Noć pod zvijezdama”,
      kao i dva koncerta u Beogradskoj Areni sa preko 40.000 fanova.
    </p>

    <h2>Humanitarni Rad</h2>
    <p>
      Članovi benda su aktivni u brojnim humanitarnim akcijama. Učestvovali su u
      mnogim dobrotvornim koncertima i događajima, podržavajući različite
      humanitarne organizacije i inicijative. Posebno su se istakli tokom
      poplava u Srbiji 2014. godine, kada su organizovali koncert za
      prikupljanje pomoći za ugrožene.
    </p>

    <h2>Popularnost i Uticaj</h2>
    <p>
      Lexington Band je stekao veliku bazu fanova, kako u Srbiji, tako i širom
      Balkana. Njihova muzika se redovno emituje na radijskim stanicama, a
      spotovi su često prikazivani na muzičkim kanalima. Njihov stil i pristup
      muzici inspirisali su mnoge mlade bendove, a njihova posvećenost kvalitetu
      i inovaciji nastavila je da privlači nove slušaoce.
    </p>

    <h2>Budućnost</h2>
    <p>
      Lexington Band nastavlja da radi na novim projektima i muzici. Njihova
      energija, kreativnost i strast prema muzici osiguravaju da će i dalje biti
      jedan od vodećih bendova na domaćoj muzičkoj sceni. Planiraju nove
      koncerte, albume i saradnje sa drugim umetnicima, čime nastavljaju da
      obogaćuju muzički pejzaž Balkana. Sa dugogodišnjom karijerom, Lexington
      Band ostavlja dubok trag u srcima svojih fanova i ostaje sinonim za
      kvalitetnu i emotivnu muziku.
    </p>
  </div>
</section>

<style>
  section {
    color: whitesmoke;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-transform: uppercase;
    z-index: 10;
  }
  img {
    position: fixed;
    z-index: 0;
    opacity: 30%;
  }
  .mob {
    display: none;
  }
  .bio-text {
    width: 40%;
    z-index: 10;
    margin-top: 7em;
  }
  h1 {
    margin-bottom: 2em;
    font-size: 1.6em;
    text-align: center;
  }
  h2,
  h3 {
    font-size: 0.8em;
    letter-spacing: 0.1em;
    font-weight: 500;
    word-spacing: 0.2em;
    margin-top: 0.4em;
  }
  p,
  li,
  span {
    font-size: 0.8em;
    letter-spacing: 0.1em;
    font-weight: 50;
    word-spacing: 0.15em;
  }
  @media (max-width: 768px) {
    .bio-text {
      width: 90%;
      margin-top: 5em;
    }
    h1 {
      margin-bottom: 2em;
    }
    .desk {
      display: none;
    }
    .mob {
      display: block;
    }
  }
</style>
