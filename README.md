# Recipe

**Recipe**는 요리와 그에 해당하는 요리 재료를 알 수 있는 프로그램입니다.

### 기본 기능
- 요리 이름
- 재료
- 재료의 양

### 기술 스택
- spring Web
- Thymeleaf
- Spring Data JPA
- mysql driver
- h2 database
- validation

### ERD
![테이블 이미지](https://github.com/KimYe-Won/inflearn-recipe/blob/main/recipe_table.png)


## API

#### 1. 레시피 작성

- **URL**: `/api/recipes`
- **METHOD**: `POST`
- **REQUEST BODY**:

<pre>
<code>
  {
  "title": "string"
}
</code>
</pre>

- **response**: `201 created`: 레시피 작성 완료

#### 2. 레시피 재료 작성

- **URL**: `/api/recipes/{recipeId}/ingredients`
- **METHOD**: `POST`
- **REQUEST BODY**:

<pre>
<code>
{
  "name": "string",
  "count": "int"
}
</code>
</pre>

- **response**: `201 created`: 레시피 재료 작성 완료
