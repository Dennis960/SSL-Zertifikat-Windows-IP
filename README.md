# SSL-Zertifikat-für-Windows

## Windows features installieren öffnen

- Internetinformationsdienste aktivieren
- Über das Startmeu Internetinformationsdienste öffnen
- Serverzertifikate -> selbstzertifiziertes Zertifikat erstellen und bennen
- Über doppelklicken auf das Zertifikat den Hash erhalten

## netsh mit Zertifikathash verwenden

```bash
netsh http add sslcert ipport=0.0.0.0:8443 certhash=24f2f770b4cac2bdcaed535385f420220b7a186e appid={df8c8073-5a4b-4810-b469-5975a9c95230}
```

- dabei ipport mit eigenem port ersetzen
- certhash mit dem Zertifikathash ersetzen
- appid mit der UUID des Programms ersetzen (Unter Vistual Studio, extras, UUID generieren)
