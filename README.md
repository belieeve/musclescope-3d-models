# MuscleScope 3D Models

3D models of the human skeleton, 20 major skeletal muscles used in strength training,
and their origin/insertion areas, prepared for the iOS app "筋肉スコープ (MuscleScope)".

These files are an **adaptation** of Z-Anatomy and BodyParts3D, and are shared under the
**Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)**.
The app's source code is not part of this repository.

## Files

| File | Contents |
|---|---|
| `MuscleScope.usdz` | Skeleton (`Skeleton`), 20 muscles (`M_<id>`), origin areas (`O_<id>`), insertion areas (`I_<id>`). Y-up, meters. |
| `MuscleScope_models.blend` | The same models as a Blender file. |
| `LICENSE` | Full text of CC BY-SA 4.0. |

Muscle ids: `pectoralis_major`, `deltoid`, `trapezius`, `latissimus_dorsi`, `biceps_brachii`,
`triceps_brachii`, `rectus_abdominis`, `external_oblique`, `erector_spinae`, `gluteus_maximus`,
`gluteus_medius`, `quadriceps`, `hamstrings`, `adductors`, `gastrocnemius`, `soleus`,
`tibialis_anterior`, `iliopsoas`, `serratus_anterior`, `rhomboids`.

## Attribution (sources)

- **BodyParts3D**, © The Database Center for Life Science (DBCLS), licensed under
  [CC BY-SA 2.1 Japan](https://creativecommons.org/licenses/by-sa/2.1/jp/).
  https://dbarchive.biosciencedbc.jp/en/bodyparts3d/download.html
- **Z-Anatomy – The libre 3D atlas of anatomy** (Kousaku Okubo, Gauthier Kervyn, Marcin Zielinski, Lluis Vinent and contributors),
  licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
  https://github.com/Z-Anatomy/Models-of-human-anatomy

Only skeleton and muscle models were used. Parts of Z-Anatomy under non-commercial licenses
(inner ear, kidney) and the Wikipedia-based definitions are **not** included.

## Changes made

- Extracted the skeleton, 20 muscles (left and right) and their attachment areas from Z-Anatomy `Startup.blend` with Blender 5.2.
- Applied modifiers, joined the parts of each muscle into one object, fixed flipped faces of mirrored parts.
- Reduced polygon count (decimation) for mobile devices.
- Re-classified each attachment area as origin or insertion according to the bone it lies on.
- Generated the insertion area of latissimus dorsi on the humerus from the contact surface between the muscle and the bone (not present in the source).
- Offset attachment areas 1.5 mm from the bone surface and assigned simple colors.

## 日本語の概要

iOSアプリ「筋肉スコープ」で使っている3Dモデル（骨格・筋トレでよく使う20筋・起始/停止の範囲）です。
Z-Anatomy と BodyParts3D（ライフサイエンス統合データベースセンター）のモデルを Blender で加工したもので、
CC BY-SA 4.0 で公開しています。表示（出典の明記）と同じライセンスでの共有を条件に、誰でも利用・改変できます。
アプリのプログラムは含みません。
