<div align=center> 
    <div style="display: flex; flex-direction: row; align-items: center; justify-content: center;">
        <img src="https://img.shields.io/badge/React-007396?style=flat&logo=React&logoColor=white" />
        <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
        <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
    </div>
    <div style="display: flex; flex-direction: row; align-items: center; justify-content: center;">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=seunghun-5945&layout=compact&theme=tokyonight"><br><br>
        <img src="https://github-readme-stats.vercel.app/api?username=seunghun-5945&show_icons=true&theme=tokyonight">
    </div>
    <img src="./profile-3d-contrib/profile-gitblock.svg" alt="3D Profile">
</div>

------- 개념정리 ---------

http: 클라이언트가 request 를 보내면 서버가 response 를 보내는거

get, post , put , delete 등이 있다.

스프링을 많이쓰는 이유: POJO는 순수 자바만 사용하는것 (파이썬 같은 타 언어가 섞이지 않음)

IoC / DI가뭔가: 제대로 못찾았으니까 내가 알아서 찾아서 정리해라

spring 과 spring boot 차이: 초기설정(DB 설정) 같은거를 몇줄로 끝낼 수 있음.

------ 무료버전 프로젝트 생성하는법 -------

spring initializr 검색 => Gradle => Java => 3.2.4 => Group이랑 Artifact , Name 을 설정하고 Dependencies 를 Spring Web 추가하고 Generate 갈기면 프로젝트파일 다운로드 받아짐
=> 압축 풀고 Intelli J 에 끌어서 실행박으면 실행됨

cmd명령어: netstat -ano 8080포트 충돌나는지 확인 만약에 같은 포트가 있어서 충돌나면 리액트 kill-port 하는것처럼 명령어로 킬 해야 하는것 같음

----- intelli J 설정 -----

annotation Processors Enable로 변경

gradle 에서 build and run 이랑 run tests using을 intellij idea 로 변경

프로젝트폴더 우클릭 설정에 Tree Appearance -> compact middle packages 체크 해제
=> src / main / java / com / test / (만든이름) / controller(만들고) / HelloController 라는 java 파일 만들어줌...

package com.test.demo.controller;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
@RequestMapping("/test")
public class HelloController {

    @GetMapping()
    public String hello2() {
        return "Hello World";
    }

    @GetMapping()
    public String hello() {
        return "Hello world";
    }
}

이러고 localhost8080/hello 들어가면
맵핑되어있는 Hello World 출력됨

다음주까지 mysql 깔아와라 ㅇㅇ.

23admin111
