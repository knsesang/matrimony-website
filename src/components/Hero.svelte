<section class="hero">
  <div class="container">
    <div class="hero-content">
      <h2>AI 기술과 사람의 섬세함을 결합한</h2>
      <h1>신뢰할 수 있는 결혼중개 플랫폼</h1>
      <p>
        인연맺음은 운영위원 주도형 커뮤니티와 AI 기반 매칭을 통해
        <br />
        한국형 결혼중개 서비스의 새로운 기준을 제시합니다.
      </p>
      <div class="cta-buttons">
        <a href="#contact" class="btn btn-primary">시작하기</a>
        <a href="#features" class="btn btn-secondary">자세히 알아보기</a>
      </div>
    </div>
    <div class="hero-stats">
      <div class="stat">
        <h3>30+</h3>
        <p>API 엔드포인트</p>
      </div>
      <div class="stat">
        <h3>7</h3>
        <p>데이터베이스 테이블</p>
      </div>
      <div class="stat">
        <h3>100%</h3>
        <p>오픈소스</p>
      </div>
    </div>
  </div>
</section>

<style>
  .hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 6rem 1rem;
    text-align: center;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .hero-content h2 {
    font-size: 1.5rem;
    font-weight: 300;
    margin-bottom: 1rem;
    opacity: 0.9;
  }

  .hero-content h1 {
    font-size: 3.5rem;
    font-weight: bold;
    margin-bottom: 1.5rem;
    line-height: 1.2;
  }

  .hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    opacity: 0.95;
    line-height: 1.6;
  }

  .cta-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
    margin-bottom: 4rem;
  }

  .btn {
    padding: 0.8rem 2rem;
    border-radius: 0.5rem;
    font-weight: 600;
    transition: all 0.3s;
    display: inline-block;
    border: none;
    cursor: pointer;
    font-size: 1rem;
  }

  .btn-primary {
    background: white;
    color: #667eea;
  }

  .btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    text-decoration: none;
  }

  .btn-secondary {
    background: transparent;
    color: white;
    border: 2px solid white;
  }

  .btn-secondary:hover {
    background: white;
    color: #667eea;
    text-decoration: none;
  }

  .hero-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin-top: 3rem;
  }

  .stat h3 {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
  }

  .stat p {
    font-size: 1rem;
    opacity: 0.9;
  }

  @media (max-width: 768px) {
    .hero {
      padding: 3rem 1rem;
    }

    .hero-content h1 {
      font-size: 2rem;
    }

    .hero-content p {
      font-size: 1rem;
    }

    .cta-buttons {
      flex-direction: column;
    }

    .btn {
      width: 100%;
    }
  }
</style>

