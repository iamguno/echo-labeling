# echo-labeling
Pandas 데이터프레임에서 'ECHO_RESULT' 열의 값들을 읽어들이고, 이 값들 중에 if 조건문 중 하나라도 포함되어 있다면, 그 해당 값을 가지는 행의 열에 값을 할당함

## 예시
코드에서 'mitral (valve) stenosis'와 유사한 단어 혹은 약어들 중 하나가 'ECHO_RESULT' 열의 값에 포함되어 있으면, 해당하는 행의 'MS' 열을 1로 할당합니다. 즉, 'mitral (valve) stenosis' 진단이 있을 경우 'MS' 열의 값을 1로 표시함

단, 코드에서 'Trivial MS', 'Mild MS', 'Mild to moderate MS', 'Mild-moderate MS'와 같은 경우에는 해당하는 행의 'MS' 열 값을 0으로 할당함. 이는 해당 진단들이 'mitral (valve) stenosis'의 정도가 매우 낮거나 경미한 경우를 나타내며, 따라서 심각한 질병으로 간주하지 않음
