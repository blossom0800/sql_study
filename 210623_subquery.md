 - SELECT 절의 SCALAR SUBQUERY(스칼라 서브쿼리) - 컬럼의 역할을 함, 반드시 단일 컬럼을 반환해야 함.
 - FROM 절의 INLINE VIEW(인라인뷰)는 하나의 테이블 역할을 함, LATERAL이라는 키워드로 JOIN 조건도 줄 수 있음. 여러 단계에 걸쳐서 데이터를 가공해서 최종 결과를 가져올 때.
 - WHERE 절의 NESTED SUBQUERY(중첩 서브쿼리), 조건절의 일부로 사용되며 서브쿼리 최종 반환값과 메인쿼리 테이블의 특정 컬럼 값을 비교할 때 사용됨

 - WITH절과 INLINE VIEW와 비슷하나
    .구조 상 INLINE VIEW는 서브쿼리를 먼저 작성해야 함. (FROM절부터 작성해야 해서)
    .WITH절은 논리 전개의 흐름대로 작성할 수 있음, 가독성 측면에서 많이 쓰임, 단 성능상 문제가 될 수 있어서 너무 남발하면 안됨.

 - Top n QUERY : ROWNUM, RANK, FETCH FIRST n ROWS(PERCENT ROWS) ONLY;
