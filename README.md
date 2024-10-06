# instgramm-nachrichten-loeschen-script
ein kleines script was nachrichten löschen kann über die console

```
const elements = document.querySelectorAll('.x1n2onr6 .x13dflua'); // eventuell ist der aber auch immer bei jedem user anders dann kann man das auch vergessen
const delay = ms => new Promise(resolve => setTimeout(resolve, ms));

async function clickElements() {
  for (let i = 0; i < elements.length; i++) {
    const element = elements[i];
    
    // Klicken auf das erste Element (div:nth-child(1))
    element.querySelector("div:nth-child(1)").click();
    await delay(800); // Warten für 500 ms

    // Klicken auf das dritte Element im Array
    document.querySelectorAll("div.x6s0dn4.x78zum5.xdt5ytf.xl56j7k")[3].click();
    await delay(500); // Wieder 500 ms warten

    // Klicken auf das zweite Element im zweiten Array
    document.querySelectorAll(".x1lliihq.x1plvlek.xryxfnj.x1n2onr6.x1ff1cvt.xatrb82.x193iq5w.xeuugli.x1fj9vlw.x13faqbe.x1vvkbs.x1s928wv.xhkezso.x1gmr53x.x1cpjm7i.x1fgarty.x1943h6x.x1i0vuye.xl565be.xo1l8bm.xkmlbd1.x1yc453h.x1tu3fi.x3x7a5m.x10wh9bi.x1wdrske.x8viiok")[2].click();
    await delay(500); // Wieder 500 ms warten

    // Klicken auf den Button
    document.querySelector("button.xjbqb8w.x1qhh985.xcfux6l.xm0m39n.x1yvgwvq.x13fuv20.x178xt8z.x1ypdohk.xvs91rp.x1evy7pa.xdj266r.x11i5rnm.xat24cr.x1mh8g0r.x1wxaq2x.x1iorvi4.x1sxyh0.xjkvuk6.xurb0ha.x2b8uid.x87ps6o.xxymvpz.xh8yej3.x52vrxo.x4gyw5p.xkmlbd1.x1xlr1w8").click();
    await delay(500); // Wieder 500 ms warten
  }
}

// Starte den Prozess
clickElements();
```

einfach in die Console kopieren und ausführen.

## Hintergrund
ich hatte das Problem das tonnen von Nachrichten an mich gesendet wurden die fragwürdigen Ihnhalt hatte. Es gibt keinerlei Möglichkeit bei Insta mehrere Nachrichten mit einmal zu löschen. Man muss immer 4 Klicks machen um eine Nachricht zu löschen. einfach mal probieren un dgern anpassen.

### was hab ich gemacht
im groben hab ich nur die selectoren gesucht und ein bisschen geschaut wie die abfolge ist und dementsprechen das script angepasst. man muss immer mal wieder neu laden und wieder starten, aber es geht. 
