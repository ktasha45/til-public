Freidburg Linear Algebra, 4th Edition
# 1.3 subspaces
## Definition
* 필드(field) F 위의 벡터 공간(vector space) V의 부분집합(subset) W는, W가 더하기(addition)와 스칼라 곱셈(scalar multiplication)의 연산(operation)을 갖는 F 위의 **벡터 공간**이라면, 필드 F 위의 **부분 공간**이라 부른다.
* 벡터 공간 V에서 V와 {0}은 부분 공간이다. 후자는 V의 **영부분공간**(zero subspace)이라고 불린다.
## Theorem
1. (Theorem 1.3) 벡터 공간 V가 있고, W는 V의 부분 집합이라고 하자. 그러면 V에서 정의된 연산에 대하여 다음 세 조건에 부합하는 경우에만 W는 V의 부분 공간이다.
   - 0 $\in$ W
   - x + y $\in$ W whenever x $\in$ W and y $\in$ W.
   - cx $\in$ W whenever c $\in$ F and x $\in$ W.
2. (Theorem 1.4) V의 부분 공간들의 교집합은 V의 부분집합이다.
# 1.4 Linear combinations and Systems of Linear equation
## Definitions
* V는 벡터 공간이고, S는 V의 진부분집합니다. 이때 벡터 v $\in$ V에 대하여 v = a1u1 + a2u2 + ··· + anun를 만족하는 유한 개의 벡터 u1, u2,...,un $\in$ S와 스칼라 a1, a2,...,an $\in$ F가 있다면 v는 S의 벡터(vectors of S)들의 선형 결합(linear combination)이다.
* V는 벡터 공간이고, S는 V의 진부분집합이다. span(S)는 S의 벡터들의 선형 결합을 모두 포함하는 집합이다. span($\phi$)는 {0}이다.
* 벡터 공간 V의 부분 집합 S는 span(S) = V일 때, V를 생성(generate)한다. 이 경우에, S의 벡터들이 V를 생성(generate or span)한다고 한다. 
## Theorem
* (Theorem 1.5) 벡터 공간 V에서 임의의 부분집합 S를 선택했을 때, span(S)은 V의 부분공간이다. 나아가, S를 포함하는 V의 부분공간은 항상 span(S) 또한 포함한다.

A subset S of a vector space V generates (or spans) V if span(S) = V. In this case, we also say that the vectors of S generate (or span) V.
# 1.5 Linear dependence and Linear independence
## definition
* 벡터 공간 V의 부분 집합 S는, a1u1 + a2u2 + ··· + anun = 0를 만족하는 유한 개의 벡터 u1, u2,...,un in S 와 scalars a1, a2,...,an, not all zero가 있다면, 선형 종속이다. 이 경우, S의 벡터들을 선형 종속이라 부른다.
* 선형 종속이 아닌, 벡터 공간의 부분 집합 S는, 선형 독립이다. 이전과 같이, S의 벡터들을 선형 독립이라 부른다.  
다음 선형 독립 집합들에 대한 사실은 모든 벡터 공간에서 성립한다.
    1. 공집합은 선형 독립이다. 선형 종속인 집합은 원소가 1개 이상 있어야 한다. (for linearly dependent sets must be nonempty)
    2. 영벡터가 아닌 벡터 하나로만 이뤄진 집합은 선형 독립이다.  
    proof. {u}가 선형 종속이라고 해보자. 그럼 0이 아닌 a에 대하여, au=0이다. 이때 u = a^−1(au) = a^−10 = 0이다. 따라서 u는 영벡터이다. 이는 가정에 위배된다. 따라서 u는 선형 종속이 아니고, 따라서 선형 독립이다.
    3. 어떤 집합의 벡터들로 영벡터를 표현(representation)하는 선형 결합이 오직 trivial한 표현밖에 없다면, 집합은 선형 독립이다.  
    *A set is linearly independent if and only if the only representations of 0 as linear combinations of its vectors are trivial representations.*
## Theorem
* (Theorem 1.6) 벡터 공간 V가 있고, S1 ⊆ S2 ⊆ V이라 하자. S1이 선형 종속이라면 S2 또한 선형 종속이다.  
*Let V be a vector space, and let S1 ⊆ S2 ⊆ V. If S1 is linearly dependent, then S2 is linearly dependent.*
* (Corollary 1 - Theorem 1.6) 벡터 공간 V가 있고, S1 ⊆ S2 ⊆ V라고 하자. S2가 선형 독립이라면, S1 또한 선형 독립이다.  
*Let V beavector space, and let S1 ⊆ S2 ⊆ V. If S2 is linearly
independent, then S1 is linearly independent.*
* (Theorem 1.7) 벡터 공간 V의 선형 독립인 부분 집합 S가 있고, V 안에 있으면서 S에는 없는 벡터 v가 있다.  이때, v $\in$ span(S)는 S ∪ {v}과 동치이다.  
*Let S be a linearly independent subset of a vector space V, and let v beavector in V that is not in S. Then S ∪ {v} is linearly dependent if and only if v ∈ span(S).*

A subset S of a vector space that is not linearly dependent
is called linearly independent. As before, we also say that the vectors of
S are linearly independent

A subset S of a vector space V is called linearly dependent
if there exist a finite number of distinct vectors u1, u2,...,un in S and scalars
a1, a2,...,an, not all zero, such that
a1u1 + a2u2 + ··· + anun = 0 .
In this case we also say that the vectors of S are linearly dependent.

# 1.6 Bases and Dimension
## Definition
* 벡터 공간 V의 기저 베타는 
A basis β for a vector space V is a linearly independent subset of V that generates V. If β is a basis for V, we also say that the vectors of β form a basis for V.