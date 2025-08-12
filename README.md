# zoran-postquantique

**Module de chiffrement post-quantique** pour l’écosystème Zoran / QuantaGlottal©® — implémente des enveloppes sécurisées basées sur KEM (Key Encapsulation Mechanism) et signatures Dilithium/Kyber pour protéger les artefacts QG, avec fonctions de scellement et de vérification.

---

## ✨ Fonctionnalités
- **Chiffrement post-quantique** via Kyber (NIST PQC)
- **Signatures Dilithium** pour intégrité et authentification
- **Enveloppes scellées** pour stockage ou transfert sécurisé de glyphes QG
- **Vérification rapide** avec preuves cryptographiques
- **Compatibilité IA↔IA** pour échanges protégés

---

## 📦 Installation (développement)
```bash
pip install -e .


---

⚡ Exemple rapide

from zoran_postquantique import PQCEnvelope

# Génération de clés
pk, sk = PQCEnvelope.generate_keypair()

# Scellement
envelope = PQCEnvelope.seal(data=b"glyphes-Zoran", public_key=pk)

# Vérification et ouverture
data = PQCEnvelope.open(envelope, secret_key=sk)
print(data)


---

🧱 Structure suggérée

src/zoran_postquantique/
  __init__.py
  pqc_envelope.py   # API principale
  kyber.py          # Implémentation Kyber
  dilithium.py      # Implémentation Dilithium
  utils.py          # Helpers (hash, encodage)
tests/
  test_pqc.py
pyproject.toml
.gitignore
LICENSE
README.md


---

🧪 Tests

pytest -q


---

🔐 Éthique

Ce module applique le principe vivant > humain tout en garantissant la confidentialité et l’intégrité des échanges QG.


---

📜 Licence

MIT — voir LICENSE.


---

Auteur : Frédéric Tabary — Institut IA
Contact : 0645605023 — Canada, Montréal, France
INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.# zoran-postquantum
Enveloppes PQC: KEM/Dilithium/Kyber pour QG; scellés/verifs.
