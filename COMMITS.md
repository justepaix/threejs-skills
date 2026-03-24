# COMMITS.md — Commit History: Three.js AI Skills

This file documents the complete commit roadmap from project initialization to v1.0 release.
Use it as a step-by-step guide when building this repo from scratch or contributing.

---

## Phase 1 — Repository Scaffolding

```
1.  chore: initial commit — empty repo with .gitignore and LICENSE

2.  chore: add README.md scaffold with ASCII art and badge placeholders

3.  chore: add AGENTS.md with repo editing guidance for AI agents

4.  chore: add CONTRIBUTING.md with PR checklist and authoring rules

5.  chore: create skills/ directory structure with empty placeholder folders

6.  chore: add .claude-plugin/ directory with plugin.json and marketplace.json

7.  chore: add .cursor-plugin/ directory with plugin.json and marketplace.json

8.  chore: add .github/copilot-instructions.md with repo-wide GSAP guidance

9.  chore: add assets/ directory with threejs-logo.svg and threejs-icon-square.svg

10. chore: add examples/ directory structure (vanilla/, react/, shaders/)
```

---

## Phase 2 — Core Skills (Foundation)

```
11. feat(core): add threejs-core SKILL.md — renderer, scene, WebGL context, render loop

12. feat(core): add resize handling, pixel ratio, tone mapping to threejs-core

13. feat(geometry): add threejs-geometry SKILL.md — built-in geometries and BufferGeometry

14. feat(geometry): add custom geometry, attributes, normals, UVs, indexed geometry to threejs-geometry

15. feat(materials): add threejs-materials SKILL.md — MeshStandardMaterial and PBR pipeline

16. feat(materials): add MAPS.md — color, normal, roughness, metalness, AO, emissive, env maps

17. feat(lighting): add threejs-lighting SKILL.md — light types, intensity, color

18. feat(lighting): add SHADOWS.md — shadow maps, bias, softness, cascade setup

19. feat(camera): add threejs-camera SKILL.md — PerspectiveCamera and OrthographicCamera

20. feat(camera): add CONTROLS.md — OrbitControls, FlyControls, PointerLockControls
```

---

## Phase 3 — Animation & Interaction

```
21. feat(animation): add threejs-animation SKILL.md — AnimationMixer and AnimationClip

22. feat(animation): add MIXER.md — keyframe tracks, morph targets, weight blending

23. feat(animation): add skinning and SkeletonHelper docs to threejs-animation

24. feat(animation): add GSAP integration patterns to threejs-animation

25. feat(loaders): add threejs-loaders SKILL.md — GLTFLoader, async loading, LoadingManager

26. feat(loaders): add GLTF.md — DRACOLoader, KTX2Loader, mesh optimization on load

27. feat(loaders): add TextureLoader, FontLoader, AudioLoader patterns to threejs-loaders

28. feat(loaders): add loading progress UI pattern and error handling to threejs-loaders
```

---

## Phase 4 — Shaders & Post-Processing

```
29. feat(shaders): add threejs-shaders SKILL.md — ShaderMaterial and RawShaderMaterial

30. feat(shaders): add GLSL.md — precision, uniforms, varyings, attributes

31. feat(shaders): add CHUNKS.md — built-in Three.js shader chunks and #include system

32. feat(shaders): add common GLSL patterns: noise, fresnel, dissolve, rim lighting

33. feat(shaders): add examples/shaders/noise.glsl — classic Perlin and simplex noise

34. feat(shaders): add examples/shaders/fresnel.glsl — fresnel rim effect

35. feat(shaders): add examples/shaders/dissolve.glsl — texture dissolve with noise

36. feat(postprocessing): add threejs-postprocessing SKILL.md — EffectComposer, RenderPass

37. feat(postprocessing): add PASSES.md — UnrealBloomPass, SSAOPass, SMAAPass, FXAAPass

38. feat(postprocessing): add pmndrs/postprocessing integration docs to PASSES.md

39. feat(postprocessing): add custom pass authoring pattern to threejs-postprocessing
```

---

## Phase 5 — Physics

```
40. feat(physics): add threejs-physics SKILL.md — physics engine overview and setup

41. feat(physics): add CANNON.md — cannon-es integration, world setup, rigid bodies

42. feat(physics): add CANNON.md — constraints, joints, collision events

43. feat(physics): add RAPIER.md — @dimforge/rapier3d-compat WASM setup

44. feat(physics): add RAPIER.md — RigidBody, Collider, joints, character controller

45. feat(physics): add examples/vanilla/physics-box.js — cannon-es drop demo

46. feat(physics): add Ammo.js integration notes and gotchas to threejs-physics
```

---

## Phase 6 — React Three Fiber

```
47. feat(react): add threejs-react SKILL.md — React Three Fiber Canvas setup

48. feat(react): add FIBER.md — useFrame, useThree, useLoader hooks

49. feat(react): add DREI.md — @react-three/drei component library patterns

50. feat(react): add Suspense and lazy-loading patterns to threejs-react

51. feat(react): add @react-three/postprocessing integration to threejs-react

52. feat(react): add examples/react/basic-r3f.jsx — minimal R3F scene

53. feat(react): add examples/react/r3f-postprocessing.jsx — bloom + SSAO demo

54. feat(react): add examples/react/r3f-physics.jsx — @react-three/rapier demo
```

---

## Phase 7 — Performance, XR & Audio

```
55. feat(performance): add threejs-performance SKILL.md — draw calls, batching overview

56. feat(performance): add PROFILING.md — Stats.js, Spector.js, Chrome GPU profiling

57. feat(performance): add instancing patterns — InstancedMesh and InstancedBufferGeometry

58. feat(performance): add LOD, frustum culling, geometry merging to threejs-performance

59. feat(performance): add texture compression — KTX2, Basis Universal, mipmap strategy

60. feat(xr): add threejs-xr SKILL.md — WebXR, VRButton, ARButton setup

61. feat(xr): add WEBXR.md — XRSession, controllers, hand tracking, hit testing

62. feat(xr): add immersive-web polyfill notes and device matrix to threejs-xr

63. feat(audio): add threejs-audio SKILL.md — AudioListener, Audio, PositionalAudio

64. feat(audio): add AudioAnalyser and Web Audio API visualization patterns
```

---

## Phase 8 — Examples & Integration

```
65. feat(examples): add examples/vanilla/basic-scene.js — canonical starter scene

66. feat(examples): add examples/vanilla/custom-shader.js — ShaderMaterial demo

67. feat(examples): add examples/vanilla/gltf-loader.js — async GLTF load with Draco

68. docs: add llms.txt skill index with names, summaries, and trigger terms

69. docs: update README.md with complete skill table and quick-reference code

70. docs: add .github/instructions/shaders.instructions.md — Copilot path-specific

71. docs: add .github/instructions/react.instructions.md — R3F Copilot guidance

72. docs: add .github/instructions/performance.instructions.md — perf Copilot hints
```

---

## Phase 9 — Testing & Quality

```
73. test: add TESTING.md with evaluation structure and manual test scenarios

74. test: add eval JSON for threejs-core — renderer setup scenario

75. test: add eval JSON for threejs-shaders — ShaderMaterial scenario

76. test: add eval JSON for threejs-react — R3F Canvas scenario

77. test: add eval JSON for threejs-physics — cannon-es drop scenario

78. fix(core): correct renderer.outputColorSpace — sRGBEncoding removed in r152

79. fix(materials): remove envMapIntensity from non-standard materials

80. fix(loaders): update import path to three/addons/ from three/examples/jsm/
```

---

## Phase 10 — Polish & Release

```
81. chore: add COMMITS.md — full commit roadmap for contributors

82. docs: add badges to README — Three.js version, license, agent compatibility

83. chore: finalize .claude-plugin/marketplace.json with correct metadata

84. chore: finalize .cursor-plugin/marketplace.json with correct metadata

85. docs: add Three.js version compatibility table to README

86. feat: add threejs-instancing sub-skill to threejs-performance

87. feat: add threejs-terrain bonus skill — heightmap, displacement, chunk loading

88. feat: add threejs-particles bonus skill — Points, PointsMaterial, GPU particles

89. docs: update CONTRIBUTING.md with v1.0 release notes and testing requirements

90. chore: tag v1.0.0 release — Three.js AI Skills stable
```

---

## Hotfix / Maintenance Commits (Post-Release)

```
91. fix(shaders): correct gl_Position assignment example in GLSL.md

92. fix(react): update useFrame signature for R3F v9

93. feat(physics): add @react-three/rapier docs to threejs-physics

94. fix(core): update toneMapping default — THREE.LinearToneMapping removed default

95. docs: clarify OrbitControls import — must come from three/addons/

96. feat(loaders): add async/await pattern for multiple concurrent GLTF loads

97. fix(postprocessing): correct EffectComposer render target format for HDR

98. feat(materials): add MeshPhysicalMaterial — transmission, thickness, iridescence

99. feat(xr): add hand tracking mesh skinning example

100. chore: tag v1.1.0 — maintenance and new features release
```

---

## Usage

Follow this roadmap sequentially when building the repo. Each commit should be:

- **Atomic**: one logical change per commit
- **Passing**: the skill works after the commit (no broken refs)
- **Described**: use the conventional commits format above

```bash
git commit -m "feat(shaders): add GLSL.md — precision, uniforms, varyings, attributes"
```
