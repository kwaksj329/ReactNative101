# ReactNative101

## 1.0 Introduction

### 1.4 Installing Requirements

React Native 앱 다운 시(apk / ipk) : Javascript <-> 운영체제 통신 인프라 또한 포함

Expo.dev : 작성한 코드 결과 앱에서 바로 확인 가능

```bash
#Install the command line tools
npm install --global expo-cli

#Create a new project
expo init my-project

#watchman install
brew update
brew install watchman
```

![rn-work](https://velog.velcdn.com/images/seoltang/post/845d144d-68c4-4d7b-be2c-d210cdd3075e/image.png)

### 1.5 How Does React Native Work

![react-native-work](https://atomate.net/wp-content/uploads/2018/11/image1.jpg)

![rn-workflow](https://media.geeksforgeeks.org/wp-content/uploads/20210713140554/GFG.png)

### 1.6 Creating The App

### 1.7 Recap

## 2.0 WEATHER APP

### 2.1 The Rules of Native

- View: container (항상 Import 하기)
- Text: text component
- 스타일 적용: StyleSheet.create() 사용 (자동완성 기능 사용 가능)
  - const styles에 바로 스타일 넣어도 됨 (자동완성 적용 안됨)

### 2.2 React Native Packages

### 2.3 Third Party Packages

- Expo SDK: API & component 제공

### 2.4 Layout System

- Flexbox로 레이아웃 생성
- Container View: 이미 Flex Container -> Flex size 부여 (비율)
  - Flex인 부모 중요, flex size 없다면 자식들이 어떤 것의 n배인지 모름
- Flex Direction 기본값: column
- 레이아웃에는 width, height 사용 금지

### 2.5 Styles

```js
#위 아래 센터
justifyContent: "center",
#왼 오 센터
alignItems: "center",
```

### 2.6 Styles part Two

- ScrollView
  - horizontal 속성
  - pagingEnabled 속성
  - showsHorizontalScrollIndicator false 시 indicator 숨김
  - contentContainerStyle 사용
- Dimensions API: 화면 크기 얻을 수 있음

```js
const { height, width } = Dimensions.get("window");
```
