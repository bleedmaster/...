# Technical Note TN-002

## Asynchronous Independent Bleed Geometry

**Project:** BleedMaster  
**Author:** Frank Wurtz  
**First publication:** July 2026  
**Status:** Public  
**Version:** 1.1

**Email:** datensicherung.mtb@gmail.com

---

# Introduction

Technical Note TN-001 introduced a new geometric approach to seamless bleed generation by preserving continuous visual appearance beyond the trim edge.

Further development of the same geometric foundation has resulted in an additional capability that significantly extends the flexibility of professional bleed generation.

BleedMaster is no longer limited to applying identical bleed behaviour around the complete page. Every page side can now operate independently while maintaining seamless visual continuity throughout the entire bleed construction.

---

# The Long-Standing Limitation

Conventional bleed generation generally applies identical processing around the complete page.

Although different bleed widths may be supported, the underlying image transformation usually remains uniform across all four sides. Independent behaviour for each page side introduces considerably greater geometric complexity, particularly in the corner regions where two independently processed bleed strips meet.

When every side is allowed to use different geometric parameters, maintaining perfectly continuous corner transitions becomes increasingly difficult. In practice this has traditionally required compromises or limitations.

---

# A New Result

BleedMaster introduces a fundamentally different geometric approach.

To the best of our knowledge, this is the first publicly documented solution capable of producing completely asynchronous bleed construction.

Each page side can independently define:

- bleed width,
- scaling percentage,
- stretching factor,
- mirroring behaviour,

without imposing any dependency on the remaining three page sides.

The corner geometry automatically adapts itself so that the complete bleed construction always remains geometrically closed while preserving continuous visual appearance.

The system therefore supports:

- independently configurable **top** bleed,
- independently configurable **bottom** bleed,
- independently configurable **left** bleed,
- independently configurable **right** bleed,
- independent scaling on every page side,
- independent stretching on every page side,
- independent mirroring on every page side,
- automatic corner reconstruction,
- seamless strip-to-corner continuity.

---

# Validation

The method has been successfully validated using independently configurable parameters for all four page sides.

## Validated Parameter Range

### Bleed Width

- **0.1 mm** to **10,000 mm** per individual page side

### Scaling

- **0.00001 %** to **250,000 %** per individual page side

All tested combinations maintained perfectly continuous transitions between bleed strips and corner geometry.

No visible discontinuities were introduced, regardless of the individual parameter values assigned to each page side.

---

# Theoretical Scalability

The underlying geometric model itself is scale-independent.

The construction remains mathematically identical regardless of the chosen dimensions or scaling factors.

Practical limits are determined only by software implementation, numerical precision and available system resources rather than by the geometry itself.

---

# Technical Disclosure

This Technical Note documents the existence of the achieved result.

The underlying geometry, mathematical principles, algorithms and implementation remain intentionally undisclosed.

Only the demonstrated capabilities and validated behaviour are presented in this publication.

---

# Conclusion

BleedMaster extends seamless bleed generation beyond traditional symmetric page-wide processing.

Every page side can now operate completely independently while the geometric engine automatically reconstructs the corner regions to preserve a fully closed and visually continuous bleed construction.

The introduction of asynchronous page-side geometry significantly expands the flexibility of professional PDF prepress workflows while intentionally withholding the underlying geometric principles for future technical publications.

---

## Keywords

**asynchronous bleed**, **independent bleed**, **asymmetric bleed**, **seamless bleed**, **corner continuity**, **strip-to-corner continuity**, **geometric bleed generation**, **scaling**, **stretching**, **mirroring**, **prepress**, **PDF production**, **RIP**, **CTP**

---

## Disclaimer

This publication documents the existence and validated capabilities of the described technology.

No part of this Technical Note discloses the underlying geometric principles, mathematical models, algorithms, implementation methods or source code used within the BleedMaster engine.

Nothing contained in this publication shall be interpreted as granting any license, permission or right to reproduce, implement, reverse engineer or derive the undisclosed technology.

The disclosed functionality is presented solely for scientific, technical and historical documentation purposes.

---

## Copyright

Copyright © 2026 Frank Wurtz.

This Technical Note may be freely copied and distributed only in its complete and unmodified form, including this copyright notice and all disclaimers.

BleedMaster is a software project developed by Frank Wurtz. All rights reserved.
