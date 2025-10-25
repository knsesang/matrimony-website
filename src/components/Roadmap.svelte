<section id="roadmap" class="roadmap">
  <div class="container">
    <h2>개발 로드맵</h2>
    <p class="subtitle">인연맺음의 성장 계획</p>

    <div class="roadmap-timeline">
      <div class="timeline-item completed">
        <div class="timeline-marker">✓</div>
        <div class="timeline-content">
          <h3>Phase 1: 백엔드 기초 (완료)</h3>
          <p>FastAPI 백엔드 구축</p>
          <ul>
            <li>30개 API 엔드포인트</li>
            <li>7개 데이터베이스 테이블</li>
            <li>JWT 인증 시스템</li>
            <li>Podman 배포 설정</li>
          </ul>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-marker">2</div>
        <div class="timeline-content">
          <h3>Phase 2: 프론트엔드 개발 (진행 중)</h3>
          <p>사용자 인터페이스 구축</p>
          <ul>
            <li>SvelteKit 관리자 대시보드</li>
            <li>Flutter 모바일 앱</li>
            <li>운영위원 투표 시스템 UI</li>
            <li>사용자 프로필 관리 UI</li>
          </ul>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-marker">3</div>
        <div class="timeline-content">
          <h3>Phase 3: AI 자동화 (계획)</h3>
          <p>지능형 기능 추가</p>
          <ul>
            <li>LLM 기반 시스템 변경 처리</li>
            <li>매칭 알고리즘 고도화</li>
            <li>자연어 처리 (NLP)</li>
            <li>이상 탐지 시스템</li>
          </ul>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-marker">4</div>
        <div class="timeline-content">
          <h3>Phase 4: 운영 고도화 (계획)</h3>
          <p>안정성과 성능 향상</p>
          <ul>
            <li>모니터링 (Prometheus, Grafana)</li>
            <li>로깅 (ELK Stack)</li>
            <li>자동화된 테스트</li>
            <li>성능 최적화</li>
          </ul>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-marker">5</div>
        <div class="timeline-content">
          <h3>Phase 5: 확장 (계획)</h3>
          <p>글로벌 서비스 확대</p>
          <ul>
            <li>다중 언어 지원</li>
            <li>국제 결제 시스템</li>
            <li>글로벌 배포</li>
            <li>고급 분석 기능</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .roadmap {
    padding: 6rem 1rem;
    background: white;
  }

  .container {
    max-width: 1000px;
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

  .roadmap-timeline {
    position: relative;
    padding: 2rem 0;
  }

  .roadmap-timeline::before {
    content: '';
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    width: 3px;
    height: 100%;
    background: #ddd;
    top: 0;
  }

  .timeline-item {
    margin-bottom: 3rem;
    position: relative;
  }

  .timeline-item:nth-child(odd) .timeline-content {
    margin-left: 0;
    margin-right: auto;
    width: 45%;
    text-align: right;
  }

  .timeline-item:nth-child(even) .timeline-content {
    margin-left: auto;
    margin-right: 0;
    width: 45%;
    text-align: left;
  }

  .timeline-marker {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    width: 50px;
    height: 50px;
    background: white;
    border: 3px solid #667eea;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: #667eea;
    font-size: 1.2rem;
    z-index: 10;
  }

  .timeline-item.completed .timeline-marker {
    background: #667eea;
    color: white;
  }

  .timeline-content {
    background: #f8f9fa;
    padding: 2rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .timeline-content h3 {
    color: #667eea;
    margin-bottom: 0.5rem;
    font-size: 1.2rem;
  }

  .timeline-content p {
    color: #666;
    margin-bottom: 1rem;
    font-size: 0.95rem;
  }

  .timeline-content ul {
    list-style: none;
    padding: 0;
  }

  .timeline-content li {
    padding: 0.4rem 0;
    color: #666;
    font-size: 0.9rem;
    border-bottom: 1px solid #ddd;
  }

  .timeline-content li:last-child {
    border-bottom: none;
  }

  .timeline-content li::before {
    content: '→ ';
    color: #667eea;
    font-weight: bold;
    margin-right: 0.5rem;
  }

  @media (max-width: 768px) {
    .roadmap {
      padding: 3rem 1rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .roadmap-timeline::before {
      left: 15px;
    }

    .timeline-item:nth-child(odd) .timeline-content,
    .timeline-item:nth-child(even) .timeline-content {
      width: 100%;
      margin-left: 60px;
      margin-right: 0;
      text-align: left;
    }

    .timeline-marker {
      left: 0;
      transform: translateX(0);
    }
  }
</style>

