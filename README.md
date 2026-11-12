# Patagonia Shield - Firmas

Base de malware Android que usa **Patagonia Shield** para detectar aplicaciones
peligrosas por su huella SHA-256.

| | |
|---|---|
| Revisión | 1 |
| Huellas | 100 |
| Generada | 2026-11-12 |
| Fuente | [MalwareBazaar](https://bazaar.abuse.ch/) (abuse.ch) |

## Cómo se verifica

- `biblioteca/hashes.txt`: una huella por línea, ordenadas, con la familia de malware.
- `biblioteca/firma.json`: firma ECDSA P-256 (SHA256withECDSA) de `hashes.txt`.

La app trae incluida la clave pública y **rechaza** cualquier base que no esté
firmada por Roma.69, que esté alterada o que sea más vieja que la instalada.

Clave pública (`ROMA69-P256-1`, SPKI en base64):

```
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAERzKWJ6FoybMcIpO4KeCDY5Lyi+815yBeISA3gUoyh3A27hGMk40wvyzLTM8ughPIK09llkZtxm03MZ4IAdAnww==
```

Datos de MalwareBazaar, publicados por abuse.ch bajo sus términos de uso justo.
