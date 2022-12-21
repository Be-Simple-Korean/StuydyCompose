# StuydyCompose
  
### Android Developer Compose 학습
> https://developer.android.com/courses/pathways/compose?hl=ko

### 정리
***
> remember = 리컴포지션에도 상태 유지
  * State 및 MutableState로 변수 선언 시 값이 변경될때마다 리컴포지션이 발생하지만 remeber를 사용하면 값이 유지된다.
  * by = .value를 사용할 필요가 없게 해주는 속성 위임
> LazyColumn = RecyclerView와 동일
             = 스크롤 할 때 새 컴포저블을 방출하고 계속 성능을 유지
             = 항목이 많은 목록을 렌더링할 때 좋음
> rememberSaveable = remember 함수는 컴포저블이 컴포지션에 유지되는 동안에만 동작을 하기때문에 화면전환이나 LazyColumn에서 값이 초기화되는 경우가 있으며,
                     이를 방지하기위해 사용.
> animateDpAsState = 애니메이션에 의해 객체가 업데이트되는 like MutableState와 같음
