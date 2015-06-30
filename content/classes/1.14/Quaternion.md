---
ID_PAGE: 3328
PG_TITLE: Quaternion
PG_VERSION: 1.14
---
##new [Quaternion](page.php?p=3328)(x, y, z, w)

Creates a new [Quaternion](page.php?p=3328)
####Parameters
 | Name | Type | Description
---|---|---|---
optional | x | number | The initial X coordinate
optional | y | number | The initial Y coordinate
optional | z | number | The initial Z coordinate
optional | w | number | The initial W coordinate
---

##Members

###x : number


The first coordinate

###y : number


The second coordinate

###z : number


The third coordinate

###w : number


The fourth coordinate



##Methods

###toString() &rarr; string
Returns a string representation of the quaternion


###asArray() &rarr; number[]
Returns an array representation of the quaternion


###equals(otherQuaternion) &rarr; boolean
Tests if two quaternion are identical

####Parameters
 | Name | Type | Description
---|---|---|---
 | otherQuaternion | [Quaternion](page.php?p=3328) | The quaternion to test against
---

###clone() &rarr; [Quaternion](page.php?p=3328)
Returns a clone of the quaternion


###copyFrom(other) &rarr; void
Copies another quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Quaternion](page.php?p=3328) | Another quaternion
---

###copyFromFloats(x, y, z, w) &rarr; void
Copies another queternion from a set of floats

####Parameters
 | Name | Type | Description
---|---|---|---
 | x | number | The X coordinate of another vector
 | y | number | The Y coordinate of another vector
 | z | number | The Z coordinate of another vector
 | w | number | The W coordinate of another vector
---

###add(other) &rarr; [Quaternion](page.php?p=3328)
Adds in another quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Quaternion](page.php?p=3328) | Another quaternion
---

###subtract(other) &rarr; [Quaternion](page.php?p=3328)
Substracts another quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Quaternion](page.php?p=3328) | Another quaternion
---

###scale(value) &rarr; [Quaternion](page.php?p=3328)
Scales a quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | value | number | @param value
---

###multiply(q1) &rarr; [Quaternion](page.php?p=3328)
Multiplies by another quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | q1 | [Quaternion](page.php?p=3328) | Another quaternion
---

###multiplyToRef(q1, result) &rarr; void
Multiplies another quaternion into a third target quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | q1 | [Quaternion](page.php?p=3328) | Another quaternion
 | result | [Quaternion](page.php?p=3328) | The target quaternion
---

###length() &rarr; number
The length of the quaternion


###normalize() &rarr; void
Normalizes the quaternion


###toEulerAngles() &rarr; [Vector3](page.php?p=3327)
Converts the quaternion into a [Vector3](page.php?p=3327) Euler angle and returns it


###toEulerAnglesToRef(result) &rarr; void
Converts the quaternion into a target [Vector3](page.php?p=3327)

####Parameters
 | Name | Type | Description
---|---|---|---
 | result | [Vector3](page.php?p=3327) | The target [Vector3](page.php?p=3327)
---

###toRotationMatrix(result) &rarr; void
Converts the quaternion into a target rotation [Matrix](page.php?p=3329) object

####Parameters
 | Name | Type | Description
---|---|---|---
 | result | [Matrix](page.php?p=3329) | The target [Matrix](page.php?p=3329)
---

###fromRotationMatrix(matrix) &rarr; void
Imports a source matrix into the current quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | matrix | [Matrix](page.php?p=3329) | The source [Matrix](page.php?p=3329)
---

###static Inverse(q) &rarr; [Quaternion](page.php?p=3328)
Returns the passed quaternion's inverse

####Parameters
 | Name | Type | Description
---|---|---|---
 | q | [Quaternion](page.php?p=3328) | The quaternion to inverse
---

###static RotationAxis(axis, angle) &rarr; [Quaternion](page.php?p=3328)
Creates a quaternion using an axis and an angle

####Parameters
 | Name | Type | Description
---|---|---|---
 | axis | [Vector3](page.php?p=3327) | The rotation axis
 | angle | number | Some angle
---

###static FromArray(array, offset) &rarr; [Quaternion](page.php?p=3328)
Creates a quaterion from agiven array

####Parameters
 | Name | Type | Description
---|---|---|---
 | array | number[] | The given array
optional | offset | number | The first index of the array to look at
---

###static RotationYawPitchRoll(yaw, pitch, roll) &rarr; [Quaternion](page.php?p=3328)
Creates a quaternion from yaw, pitch and roll values

####Parameters
 | Name | Type | Description
---|---|---|---
 | yaw | number | The yaw rotation
 | pitch | number | The pitch rotation
 | roll | number | The roll rotation
---

###static RotationYawPitchRollToRef(yaw, pitch, roll, result) &rarr; void
Creates a quaternion from yaw, pitch and roll values and put it in the target quaternion

####Parameters
 | Name | Type | Description
---|---|---|---
 | yaw | number | The yaw rotation
 | pitch | number | The pitch rotation
 | roll | number | The roll rotation
 | result | [Quaternion](page.php?p=3328) | The target quaternion
---

###static Slerp(left, right, amount) &rarr; [Quaternion](page.php?p=3328)
Performs a spherical linear interpolation between two quaternions

####Parameters
 | Name | Type | Description
---|---|---|---
 | left | [Quaternion](page.php?p=3328) | interpolation start quaternion
 | right | [Quaternion](page.php?p=3328) | interpolation end quaternion
 | amount | number | Weighting factor
---