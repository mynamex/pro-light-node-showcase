# ESP NotebookLM Context

Generated at: 2026-05-18T02:48:37

## Hedef

ESP32 node production lighting fixture gibi davranacak.

Ana sorumlulukları:

- BLE Mesh node/proxy/relay runtime
- Vendor packet RX
- Protocol decode
- Time sync
- Scheduled command queue
- Render/effect/fan/thermal/safety/telemetry layers

## Şu anki kritik konu

Legacy RGB group testi PASS verdi.

V2 scheduled effect testinde:
- TIME_SYNC görüldü
- V2 group effect gönderildi
- Bir node scheduled/apply yaptı
- Diğer node packet aldı ama scheduler reject etti

Bu yüzden ilk odak:

Packet ulaşıyor mu?
Decode doğru mu?
Time sync fresh mi?
startAtMs geçmişte mi?
cueId duplicate mi?
Queue dolu mu?
Scheduler neden reject ediyor?

## NotebookLM’den beklenen

Kod yazmasın.
Önce flow ve reject ihtimallerini dosya kanıtıyla çıkarsın.

