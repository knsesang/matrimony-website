<section id="features" class="features">
  <div class="container">
    <h2>핵심 특징</h2>
    <p class="subtitle">인연맺음이 제공하는 혁신적인 기능들</p>

    <div class="features-grid">
      <div class="feature-card">
        <div class="icon">🤖</div>
        <h3>AI 기반 매칭</h3>
        <p>
          사용자의 프로필, 가치관, 선호도를 분석하여
          최적의 상대를 추천합니다.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">🏢</div>
        <h3>운영위원 주도형</h3>
        <p>
          여러 운영위원이 투표를 통해 서비스 개선에
          직접 참여합니다.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">🔐</div>
        <h3>신뢰성 높은 인증</h3>
        <p>
          민감 정보를 단계별로 인증하여
          회원의 신뢰도를 확보합니다.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">📱</div>
        <h3>모바일 우선 설계</h3>
        <p>
          Flutter 모바일 앱을 통한
          편리한 사용자 경험을 제공합니다.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">⚡</div>
        <h3>트래픽 분산</h3>
        <p>
          여러 운영위원 서버를 통한
          확장 가능한 아키텍처입니다.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">🌍</div>
        <h3>확장 가능성</h3>
        <p>
          향후 일부 로직을 회사 서버로 분리하여
          더욱 강화된 기능을 제공할 수 있습니다.
        </p>
      </div>
    </div>
  </div>
</section>

<style>
  .features {
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

  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
  }

  .feature-card {
    background: white;
    padding: 2rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    transition: all 0.3s;
    text-align: center;
  }

  .feature-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
  }

  .icon {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .feature-card h3 {
    font-size: 1.3rem;
    margin-bottom: 0.8rem;
    color: #333;
  }

  .feature-card p {
    color: #666;
    line-height: 1.6;
    font-size: 0.95rem;
  }

  @media (max-width: 768px) {
    .features {
      padding: 3rem 1rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .features-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

