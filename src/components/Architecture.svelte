<section id="architecture" class="architecture">
  <div class="container">
    <h2>시스템 아키텍처</h2>
    <p class="subtitle">운영위원 트래픽 분산 기반의 확장 가능한 구조</p>

    <div class="architecture-diagram">
      <div class="diagram-section">
        <h3>모바일 앱 사용자</h3>
        <div class="diagram-box">
          <p>Flutter 모바일 앱</p>
        </div>
      </div>

      <div class="arrow">↓</div>

      <div class="diagram-section">
        <h3>운영위원 서버들</h3>
        <div class="diagram-boxes">
          <div class="diagram-box">운영위원 A<br />(VPS)</div>
          <div class="diagram-box">운영위원 B<br />(VPS)</div>
          <div class="diagram-box">운영위원 C<br />(VPS)</div>
        </div>
        <p class="description">
          각 운영위원이 자신의 VPS에 FastAPI 백엔드 배포<br />
          모든 비즈니스 로직 포함 (인증, 매칭, 검색)
        </p>
      </div>

      <div class="arrow">↓</div>

      <div class="diagram-section">
        <h3>중앙 서버</h3>
        <div class="diagram-box">
          <p>PostgreSQL 데이터베이스</p>
          <p style="font-size: 0.9rem; margin-top: 0.5rem;">+ SvelteKit 관리자 대시보드</p>
        </div>
        <p class="description">
          단일 소스 오브 트루스<br />
          운영위원 투표 시스템, 요청 승인 관리
        </p>
      </div>
    </div>

    <div class="architecture-details">
      <div class="detail-card">
        <h4>운영위원 VPS</h4>
        <ul>
          <li>FastAPI 백엔드</li>
          <li>Nginx 리버스 프록시</li>
          <li>Redis 캐싱</li>
          <li>모든 비즈니스 로직</li>
        </ul>
      </div>

      <div class="detail-card">
        <h4>중앙 서버</h4>
        <ul>
          <li>PostgreSQL 데이터베이스</li>
          <li>Redis 세션 관리</li>
          <li>SvelteKit 대시보드</li>
          <li>운영위원 투표 시스템</li>
        </ul>
      </div>

      <div class="detail-card">
        <h4>주요 특징</h4>
        <ul>
          <li>트래픽 분산</li>
          <li>확장 가능한 구조</li>
          <li>데이터 동기화</li>
          <li>고가용성</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<style>
  .architecture {
    padding: 6rem 1rem;
    background: white;
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

  .architecture-diagram {
    background: #f8f9fa;
    padding: 3rem;
    border-radius: 0.8rem;
    margin-bottom: 3rem;
    text-align: center;
  }

  .diagram-section {
    margin: 2rem 0;
  }

  .diagram-section h3 {
    color: #667eea;
    margin-bottom: 1rem;
    font-size: 1.2rem;
  }

  .diagram-box {
    background: white;
    border: 2px solid #667eea;
    border-radius: 0.5rem;
    padding: 1.5rem;
    margin: 1rem auto;
    max-width: 400px;
    color: #333;
    font-weight: 500;
  }

  .diagram-boxes {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
    gap: 1rem;
    max-width: 600px;
    margin: 0 auto;
  }

  .diagram-boxes .diagram-box {
    margin: 0;
    padding: 1rem;
    font-size: 0.9rem;
  }

  .arrow {
    font-size: 1.5rem;
    color: #667eea;
    margin: 1rem 0;
  }

  .description {
    font-size: 0.9rem;
    color: #666;
    margin-top: 0.5rem;
    line-height: 1.5;
  }

  .architecture-details {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
  }

  .detail-card {
    background: #f8f9fa;
    padding: 2rem;
    border-radius: 0.8rem;
    border-left: 4px solid #667eea;
  }

  .detail-card h4 {
    color: #667eea;
    margin-bottom: 1rem;
    font-size: 1.1rem;
  }

  .detail-card ul {
    list-style: none;
    padding: 0;
  }

  .detail-card li {
    padding: 0.5rem 0;
    color: #666;
    border-bottom: 1px solid #ddd;
  }

  .detail-card li:last-child {
    border-bottom: none;
  }

  @media (max-width: 768px) {
    .architecture {
      padding: 3rem 1rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .architecture-diagram {
      padding: 1.5rem;
    }

    .diagram-boxes {
      grid-template-columns: 1fr;
    }
  }
</style>

