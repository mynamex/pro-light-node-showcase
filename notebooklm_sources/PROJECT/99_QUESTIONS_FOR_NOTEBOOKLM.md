# QUESTIONS FOR NOTEBOOKLM

## Android Provision / Network Soruları

1. Provision flow hangi dosyada başlıyor ve hangi dosyada bitiyor?
2. Provision sırasında scan pause/resume deterministic mi?
3. Provision sonrası proxy bağlantısını kim sahipleniyor?
4. Config flow provision’dan sonra otomatik ve kontrollü mü başlıyor?
5. Config işlemi ACK/state-driven mı yoksa delay/time-based mi?
6. WorkScreen yanlışlıkla config tetikliyor mu?
7. PresenceService ile AutoReconnectService birbirine fazla bağlı mı?
8. ProxySelectionPolicy production için yeterli mi?
9. MeshController çok fazla sorumluluk alıyor mu?
10. Sidus-like architecture için en küçük güvenli refactor nedir?

## ESP Scheduler / Runtime Soruları

1. V2 packet vendor callback’ten hangi katmanlara ilerliyor?
2. Decode failure ile scheduler reject logları net ayrılmış mı?
3. Scheduler hangi şartlarda reject ediyor?
4. Reject reason explicit loglanıyor mu?
5. startAtMs absolute timestamp mı, relative delay mi?
6. ESP local clock compare signed/unsigned problemine açık mı?
7. cueId duplicate protection nasıl çalışıyor?
8. Queue thread-safe mi?
9. Processor ve render engine aynı task/core üzerinde mi?
10. TIME_SYNC fresh değilse scheduler ne yapıyor?

## Cevap Formatı

Lütfen şu formatla cevap ver:

- Flow özeti
- Ownership haritası
- Riskli coupling noktaları
- En olası bug adayları
- Minimal test önerisi
- Kod yazmadan önce görülmesi gereken loglar
