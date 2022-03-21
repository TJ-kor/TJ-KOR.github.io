---
layout: post
title: GitHub blog 시작하기
subtitle: ruby, jekyll 설치 및 테마 적용
categories: jekyll
tags: [jekyll, Github]
sitemap :
  changefreq : weekly
  priority : 0.9
---

## 시작하기

 안녕하세요. 이 포스트에서는 Github와 Jekyll을 이용한 github.io 작성을 소개하겠습니다.
 다양한 블로그 플랫폼들이 있지만, 자유로운 사용자화와 Git을 이용한 관리의 장점이 있다고 생각하여 Github를 선택하게 되었습니다.

 진입 장벽이 다소 있다고 생각을 합니다. 그렇지만 웹과 관련한 경험이 없는 분들에게는 좋은 경험이 될 수도 있다고 생각을 합니다. 

 소스 코드의 게시도 깔끔하다고 생각합니다.
 예시 코드 )
```cpp
void insert(const char* key) {
    if (*key == '\0') {
        finish = true;
    } else {
        int idx = *key - 'A';
        if (!next[idx])
            next[idx] = new Trie();
        next[idx]->insert(key + 1);
    }
}
```

 다시 본론으로 돌아와서 github.io 작성을 위해 Repository를 생성하고, ruby를 이용한 Jekyll을 설치하는 과정을 소개 하겠습니다.
 그리고 온라인에 공유되고 있는 테마 소스를 받아서 적용 해보도록 하겠습니다.

Tips:
* 아래의 링크와 같이 Github에서 공식적으로 소개하는 작성 방법도 있습니다.
* <https://pages.github.com/>


## Github Repository

<https://www.github.com>


## Ruby 

<https://rubyinstaller.org/>

``` console
> ruby -v
``` 

## Jekyll

### 설치 및 테스트

``` console
> gem install jekyll bundle
> jekyll -v
> bundle -v
```

``` console
> jekyll new ./
> bundle install
```
``` console
> bundle exec jekyll serve
```

### 테마 적용하기

``` console
> git add . 
> git commit -m "any commit messages"
> git push
```

