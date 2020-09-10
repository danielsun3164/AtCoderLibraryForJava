# クラスMathLib

数学的アルゴリズム詰め合わせです. 整数計算に関する様々なアルゴリズムが入っています.

## crt
```java
public static long[] crt(long[] r, long[] m)
```

同じ長さの配列 r, m を渡します. この配列の長さをn としたとき,
$$ x \equiv r[i] \mod m[i] $$ を解きます.

答えは存在するならば $ y, z (0 \leq y < z = lcm(m))$ を用いて $ x \equiv y \mod z $の形で書けることが知られています.

この関数の返り値は, yとzをこの順に格納した長さ2の配列です.

答えがない場合は [0,0] を返します. n=0 のときは [0,1] を返します.

## floor_sum
```java
public static long floor_sum(long n, long m, long a, long b)
```

$ \signa_{i=0}^{n-1} floor(\frac{a*i+b}{m}) $を返します.