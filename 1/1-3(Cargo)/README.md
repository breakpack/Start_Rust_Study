# Cargo 사용  
- 카고(Cargo)는 러스트 빌드 시스템 및 패키지 매니저

## 1. 설치  
- 는 이미 되어 있을것(설치 확인)
```
$ cargo --version
```

## 2. 사용 - cargo 프로젝트 생성
```
$ cargo new hello_cargo --bin
$ cd hello_cargo
```
- hello_cargo라는 실행가능한 바이너리 생성(--bin인자를 이용)


## 3. Cargo.toml
- TOML (Tom’s Obvious, Minimal Language) 포맷으로 작성되었는데, 이것이 Cargo의 환경설정 포맷임
- [package]은 이후의 문장들이 패키지 환경설정이라는 것을 나타내는 섹션의 시작지점
- [dependencies]은 프로젝트의 의존성들의 리스트를 적을 수 있는 섹션의 시작점

- Rust의 코드 패키지는 크레이트(Crate)라고 부름

- 코딩할때 코드를 src 디렉토리로 옮기고 적합한 Cargo.toml 파일을 생성
```
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2021"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
```

## 4. build + excute  
**build** 
```
$ cargo build
```
- build는 Cargo.toml파일이 있는 디렉토리에서 실행 -> target/debug/hello_cargo

**excute**  
```
$ cargo run
```
- ./hello_cargo로도 실행가능

**compile check**  
```
$ cargo check
```
- 실행파일 생성은 안함

**release build**  
```
$ cargo build --release
```