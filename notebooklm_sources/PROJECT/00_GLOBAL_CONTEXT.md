# PROJECT GLOBAL CONTEXT

Generated at: 2026-05-18T02:48:37

## Proje

Pro-Light BLE Mesh

Android + ESP32 tabanlı Sidus Link benzeri cinema lighting control sistemi.

## Ana hedef

Birden fazla ESP32 ışık node’u:

- stabil provision edilecek
- ACK/state-driven config alacak
- group address 0xC000 dinleyecek
- Android üzerinden proxy node aracılığıyla kontrol edilecek
- online/offline presence ile izlenecek
- time sync ile scheduled cue/effect komutlarını aynı anda uygulayacak
- recovery/state/telemetry mekanizmalarına sahip olacak

## Güncel teknik sonuç

Legacy group RGB PASS:
- Mesh tamamen ölü değil.
- Group subscription tamamen bozuk görünmüyor.
- Proxy forwarding en azından legacy komutta çalışıyor.

V2 scheduled effect FAIL:
- Sorun artık sadece packet ulaşmıyor değil.
- Packet ulaşıp scheduler tarafından reddediliyor olabilir.

## Ana debugging ilkesi

Varsayıma göre kod yazma.
Önce mevcut dosya ve logdan flow çıkar.
Sonra minimal değişiklik yap.
Her değişikliği test sonucu ile not al.

