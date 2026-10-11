Project Turul Reforge Azeroth 1.3.0

Önálló magyarítás AzerothCore / World of Warcraft 3.3.5a (enUS) klienshez.

Fő funkciók:
- Stabil WotLK 3.3.5a quest-ID felismerő mag a működő QuestTradutor motor alapján.
- Teljes magyar QuestData, Gossip, Tooltip, Book és Bubble adatbázis betöltése.
- Küldetések és NPC/Gossip párbeszédek magyarítása.
- Vendor- és egyéb item-tooltipok magyarítása a hash-alapú tooltip adatbázissal.
- Könyvek és olvasható tárgyak fordítása ITEM_TEXT_READY és GET_ITEM_INFO_RECEIVED eseményekkel.
- Első megnyitáskor aszinkron item-info betöltés kezelése; C_Timer.After használata, 3.3.5a-n pedig biztonságos OnUpdate tartalék.
- Chat buborék fordítás a WorldFrame FontString elemeinek megtisztításával és hash-alapú kereséssel.
- WoW 3.3.5a Interface Options panel az AddOns fül alatt.
- Öt külön kapcsoló: Küldetés, Gossip, Könyv, Tooltip, Chat buborék.
- A beállítások a HuncraftSettings SavedVariables táblában maradnak meg.
- /ptra és /turul parancsok azonnal megnyitják a Project Turul beállításait.
- A modulok futás közben minden alkalommal ellenőrzik a saját HuncraftSettings kapcsolójukat.
- A canonical $N, $C/$c, $R/$r, $B és $Gmale:female; helyőrzők megmaradnak.
- UTF-8, BOM nélkül.

Telepítés:
1. Töröld a korábbi ProjectTurulReforgeAzeroth mappát.
2. Másold ezt a ProjectTurulReforgeAzeroth mappát az Interface\AddOns könyvtárba.
3. Indítsd újra a klienst.
4. A Beállítások -> AddOns -> Project Turul: Reforge Azeroth alatt külön kapcsolható az öt fordítási modul.

Megjegyzés:
Az NPCData.lua szándékosan nem tartalmaz kitalált NPC-adatokat. A meglévő működő QuestTradutor/Gossip és tooltip adatbázisok maradnak az addon hiteles fordítási forrásai.
