# core: cosine-distance-test

*Community 12 | 3 files | cohesion 1.00*

## Definition

This community groups 3 file(s) rooted at `core` with dominant language cpp (cohesion 1.00). Central symbols: `COSINE_DISTANCE_H_`, `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`, `SUBCASE`, `TEST_CASE`, `cosine_distance`. Core file: `core/cosine-distance-test.cpp` (8 symbols). Documented purpose: Computes cosine distance between two vectors: 1 - (a·b)/(||a||*||b||). Matches scipy.spatial.distance.cdist(..., metric="cosine")[0,0]. Throws std::invalid_argu.

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/cosine-distance-test.cpp` | cpp | testing | 8 | no |
| `core/cosine-distance.cpp` | cpp | utility | 1 | no |
| `core/cosine-distance.h` | h | utility | 2 | yes |

## Key Symbols

- `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, `core/cosine-distance-test.cpp:5`) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- `TEST_CASE` (function, `core/cosine-distance-test.cpp:8`) `TEST_CASE("cosine-distance")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:9`) `SUBCASE("identical vectors give zero distance")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:15`) `SUBCASE("orthogonal vectors give distance one")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:21`) `SUBCASE("opposite vectors give distance two")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:27`) `SUBCASE("mismatched length throws")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:33`) `SUBCASE("zero vector gives zero distance")`
- `SUBCASE` (function, `core/cosine-distance-test.cpp:39`) `SUBCASE("matches scipy implementation")`
- `cosine_distance` (function, `core/cosine-distance.cpp:6`) `float cosine_distance(const std::vector<float>& a,                       const s`
- `COSINE_DISTANCE_H_` (macro, `core/cosine-distance.h:2`) `#define COSINE_DISTANCE_H_`
- `cosine_distance` (function, `core/cosine-distance.h:9`) `float cosine_distance(const std::vector<float>& a, const std::vector<float>& b);` - Computes cosine distance between two vectors: 1 - (a·b)/(\|\|a\|\|*\|\|b\|\|). Matches scipy.spatial.distanc

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 2
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- [INFERRED] shares_context community 0 <-> 12 (strength 0.5): Inferred shared context (language cpp and layer utility) with no import path between community 0 (core: moonshine-cpp) and community 12 (core: cosine-distance-test).

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 2 file(s) lack file-level docs (e.g. `core/cosine-distance-test.cpp`)? What purpose do they serve?
- What would break if the most connected file in core: cosine-distance-test changed?
- Should core: cosine-distance-test be split, given cohesion 1.00?

## Sources

- `core/cosine-distance-test.cpp`
- `core/cosine-distance.cpp`
- `core/cosine-distance.h`
