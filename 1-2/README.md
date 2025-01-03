# Hello! World!!

## 1. Test Dir 생성
```
$ mkdir hello_world
$ cd hello_world
```

## 2. Hello! World!!
```
//main.rs

fn main() {
  println!("Hello, world!");
}
```
- main 함수를 사용 <- 가장 먼저 실행됨
- println! <- ```!```가 붙으면 함수가 아니라 매크로 호출 코드 (19장에서 다룸)

## 3. 실행시키기
```
$ rustc main.rs
$ ./main
```
- rustc main.rs 를 통해서 Clang과 비슷하게 컴파일