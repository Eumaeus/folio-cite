Highlighting groups for various occasions
-----------------------------------------

Syntax highlighting groups
--------------------------
# Alignment of Sub-Referenced CTS-URNs to “Tokenized” Editions
	
## Example URNs
	
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.1`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.2`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.3`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.4`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.5`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.6`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.7`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.8`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:2.6`
	
Are "realignments" of:

- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@ὦ[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τέκνα[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@,[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@Κάδμου[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τοῦ[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@πάλαι[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@νέα[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τροφή[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:2@θοάζετε[1]`

## Possibilities

### Leaf-Node Citations

- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.1`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.2`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@ὦ[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τέκνα[1]`

### Range Citations

- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.1-1.2`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1.2-2.6`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1-2`
- `urn:cts:greekLit:tlg0011.tlg004.fu04:1-2.6`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@ὦ-1@τέκνα[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τέκνα-2@θοάζετε[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1-1@τέκνα[1]`
- `urn:cts:greekLit:tlg0011.tlg004.fu01:1@τέκνα-2[1]`

### In other words

Citing the base text:

- Leaf-node with sub-ref.
- Range with 2 sub-refs.
- Range with 1 sub-ref.

Citing the Refactored text:

- Leaf-node (token)
- Range (token-to-token)
	- May be a refactoring of a leaf node in the base-text.
- Range (containingNode-to-token)
	- May be a refactoring of a leaf node in the base-text.
- Range (token-to-containingNode)
	- May be a refactoring of a leaf node in the base-text.


## CTS Service

- We only care about GetPassage, GetPassagePlus.
- We only need to worry about stuff with subrefs.

### In API

1. Get URN. Does it have a subref?
