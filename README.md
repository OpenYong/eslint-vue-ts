# @yong-lee/eslint-config-vue

Vue.js 프로젝트에서 TypeScript와 함께 사용할 수 있는 ESLint 구성 패키지입니다.

## 설치

```bash
npm install --save-dev @yong-lee/eslint-config-vue
```

## 사용 방법
이 ESLint 구성을 Vue.js 프로젝트에서 사용하려면 프로젝트 루트에 ESLint 구성 파일을 만들고 다음과 같은 내용을 추가하세요 (예: `.eslintrc.js` 또는 `.eslintrc.json`):

```
module.exports = {
  extends: [
    "@yong-lee/eslint-config-vue"
  ],
  // 프로젝트별 구성 또는 오버라이드를 추가하세요
};
```

## Configuration
이 구성은 다음 ESLint configuration(구성)을 확장합니다:

- eslint:recommended
- plugin:@typescript-eslint/recommended
- plugin:vue/vue3-essential
- plugin:prettier/recommended
- plugin:vue/vue3-strongly-recommended
- @vue/eslint-config-typescript
- @vue/eslint-config-prettier/skip-formatting
들여쓰기, 줄 바꿈, 따옴표 등에 대한 규칙이 포함되어 있습니다. 프로젝트의 ESLint 구성 파일에서 이러한 규칙을 사용자 정의하거나 오버라이드할 수 있습니다.

## Example Configuration (구성 예시)
다음은 사용자 지정 ESLint 구성 파일의 예입니다. 프로젝트별 규칙이나 오버라이드를 추가하세요:

```
module.exports = {
  extends: [
    "@yong-lee/eslint-config-vue"
  ],
  rules: {
    // 프로젝트별 규칙이나 오버라이드를 추가하세요
    'vue/attribute-hyphenation': ['error', 'never']
  },
};
```

## License

이 프로젝트는 MIT 라이선스를 따릅니다. 자세한 내용은 [라이선스 파일](LICENSE)을 참조하세요.
