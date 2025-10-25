<section id="technology" class="technology">
  <div class="container">
    <h2>기술 스택</h2>
    <p class="subtitle">최신 기술을 활용한 견고한 구축</p>

    <div class="tech-grid">
      <div class="tech-category">
        <h3>백엔드</h3>
        <div class="tech-items">
          <div class="tech-item">
            <span class="tech-name">Python 3.11</span>
            <span class="tech-desc">프로그래밍 언어</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">FastAPI</span>
            <span class="tech-desc">웹 프레임워크</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">SQLAlchemy</span>
            <span class="tech-desc">ORM</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">PostgreSQL</span>
            <span class="tech-desc">데이터베이스</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Redis</span>
            <span class="tech-desc">캐싱</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">JWT</span>
            <span class="tech-desc">인증</span>
          </div>
        </div>
      </div>

      <div class="tech-category">
        <h3>배포 & 인프라</h3>
        <div class="tech-items">
          <div class="tech-item">
            <span class="tech-name">Docker</span>
            <span class="tech-desc">컨테이너</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Podman</span>
            <span class="tech-desc">컨테이너 런타임</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Nginx</span>
            <span class="tech-desc">리버스 프록시</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Ubuntu</span>
            <span class="tech-desc">운영 체제</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Let's Encrypt</span>
            <span class="tech-desc">SSL 인증서</span>
          </div>
        </div>
      </div>

      <div class="tech-category">
        <h3>프론트엔드</h3>
        <div class="tech-items">
          <div class="tech-item">
            <span class="tech-name">SvelteKit</span>
            <span class="tech-desc">웹 프레임워크</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Flutter</span>
            <span class="tech-desc">모바일 앱</span>
          </div>
          <div class="tech-item">
            <span class="tech-name">Svelte</span>
            <span class="tech-desc">UI 라이브러리</span>
          </div>
        </div>
      </div>
    </div>

    <div class="api-stats">
      <div class="stat">
        <h4>30+</h4>
        <p>API 엔드포인트</p>
      </div>
      <div class="stat">
        <h4>7</h4>
        <p>데이터베이스 테이블</p>
      </div>
      <div class="stat">
        <h4>5</h4>
        <p>라우터 모듈</p>
      </div>
      <div class="stat">
        <h4>3</h4>
        <p>사용자 유형</p>
      </div>
    </div>
  </div>
</section>

<style>
  .technology {
    padding: 6rem 1rem;
    background: #f8f9fa;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  h2 {
    font-size: 2.5rem;
    text-align: center;
    margin-bottom: 1rem;
    color: #333;
  }

  .subtitle {
    text-align: center;
    color: #666;
    font-size: 1.1rem;
    margin-bottom: 3rem;
  }

  .tech-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin-bottom: 3rem;
  }

  .tech-category {
    background: white;
    padding: 2rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .tech-category h3 {
    color: #667eea;
    margin-bottom: 1.5rem;
    font-size: 1.3rem;
    border-bottom: 2px solid #667eea;
    padding-bottom: 0.5rem;
  }

  .tech-items {
    display: grid;
    gap: 1rem;
  }

  .tech-item {
    display: flex;
    flex-direction: column;
    padding: 1rem;
    background: #f8f9fa;
    border-radius: 0.5rem;
    border-left: 3px solid #667eea;
  }

  .tech-name {
    font-weight: 600;
    color: #333;
    font-size: 0.95rem;
  }

  .tech-desc {
    font-size: 0.85rem;
    color: #666;
    margin-top: 0.3rem;
  }

  .api-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1.5rem;
    text-align: center;
  }

  .stat {
    background: white;
    padding: 2rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .stat h4 {
    font-size: 2rem;
    color: #667eea;
    margin-bottom: 0.5rem;
  }

  .stat p {
    color: #666;
    font-size: 0.9rem;
  }

  @media (max-width: 768px) {
    .technology {
      padding: 3rem 1rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .tech-grid {
      grid-template-columns: 1fr;
    }

    .api-stats {
      grid-template-columns: repeat(2, 1fr);
    }
  }
</style>

