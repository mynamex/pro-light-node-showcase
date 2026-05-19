# ANDROID NotebookLM Context

Generated at: 2026-05-18T02:48:37

## Hedef

Android uygulama Sidus Link benzeri production kontrol merkezi olacak.

Ana sorumlulukları:

- Provisioning lifecycle
- Config lifecycle
- Proxy selection/reconnect
- Presence based online/offline tracking
- Group/unicast vendor command sending
- Time sync and scheduled cue orchestration
- State authority / recovery

## Önemli Mimari Kural

WorkScreen config yapmamalı.

WorkScreen sadece kullanıcı aksiyonunu almalı.
Gerçek iş akışı şu katmanlarda olmalı:

UI
↓
MeshCommandService
↓
TimeSyncService / CueManager
↓
MeshCommander
↓
MeshController

## NotebookLM’den beklenen

Kod yazmasın.
Önce flow çıkarsın:

- Provision nerede başlıyor, nerede bitiyor?
- Config kim tarafından tetikleniyor?
- Proxy reconnect ile presence birbirine karışmış mı?
- UI iş mantığı taşıyor mu?
- Sidus-like mimari için ownership doğru mu?

