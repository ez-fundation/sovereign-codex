# Symbeon Protocol: Technical Specification v0.2.0

## 1. The Symbeon Intent Schema
The core of the protocol is the **Isomorphic Intent**. This JSON structure serves as the contract between the Archaeologist (AION) and the Generator (EZ-Studios).

### 1.1 structure
```json
{
    "id": "intent_<uuid>",
    "categoria": "Mapa | Actor | Item | Physics | VFX | UI",
    "descricaoNatural": "Natural language synthesis of the findings",
    "parametros": {
        "source_binary": "filename",
        "source_offset": "hex_offset",
        "entropy": "float",
        "estetica": "Dynamic Aesthetic Label",
        "tags": ["keyword1", "keyword2"]
    },
    "metadados": {
        "autorId": "AION_ENGINE",
        "seed": "extraction_seed",
        "hashGeracao": "unique_hash"
    }
}
```

## 2. Isomorphic Mapping Principles
1.  **Conservation of Entropy:** The complexity of the output world must be proportional to the entropy of the source binary.
2.  **Aesthetic Continuity:** Use pattern-scoring to derive visual themes (e.g., High Complexity -> Cybernetic-Legacy).
3.  **Algorithmic Injection:** Eon-Chess logic must be injected into the generated NPCs to maintain "Pure Logic" behavior.

## 3. Integration Interface
AION exports to `<ROOT>/AION_REPORTS/aion_intent.json`.
EZ-Studios monitors this path to trigger the **Seed-to-World** pipeline.

---
*EZ-Fundation Technical Standards*
