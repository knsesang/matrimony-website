<script>
  let formData = {
    name: '',
    email: '',
    message: ''
  };

  let submitted = false;

  function handleSubmit(e) {
    e.preventDefault();
    // 실제 구현에서는 백엔드로 전송
    console.log('Form submitted:', formData);
    submitted = true;
    setTimeout(() => {
      submitted = false;
      formData = { name: '', email: '', message: '' };
    }, 3000);
  }
</script>

<section id="contact" class="contact">
  <div class="container">
    <h2>문의하기</h2>
    <p class="subtitle">인연맺음에 대해 더 알고 싶으신가요?</p>

    <div class="contact-content">
      <div class="contact-info">
        <div class="info-item">
          <h3>📧 이메일</h3>
          <p><a href="mailto:info@matrimony.com">info@matrimony.com</a></p>
        </div>
        <div class="info-item">
          <h3>📞 전화</h3>
          <p><a href="tel:+82-2-1234-5678">+82-2-1234-5678</a></p>
        </div>
        <div class="info-item">
          <h3>🌐 웹사이트</h3>
          <p><a href="https://github.com/your-username/matrimony-platform" target="_blank">GitHub 저장소</a></p>
        </div>
        <div class="info-item">
          <h3>📍 위치</h3>
          <p>서울, 대한민국</p>
        </div>
      </div>

      <form on:submit={handleSubmit} class="contact-form">
        {#if submitted}
          <div class="success-message">
            <p>✓ 메시지가 전송되었습니다. 감사합니다!</p>
          </div>
        {:else}
          <div class="form-group">
            <label for="name">이름</label>
            <input
              type="text"
              id="name"
              bind:value={formData.name}
              required
              placeholder="이름을 입력하세요"
            />
          </div>

          <div class="form-group">
            <label for="email">이메일</label>
            <input
              type="email"
              id="email"
              bind:value={formData.email}
              required
              placeholder="이메일을 입력하세요"
            />
          </div>

          <div class="form-group">
            <label for="message">메시지</label>
            <textarea
              id="message"
              bind:value={formData.message}
              required
              placeholder="메시지를 입력하세요"
              rows="5"
            ></textarea>
          </div>

          <button type="submit" class="btn-submit">전송하기</button>
        {/if}
      </form>
    </div>
  </div>
</section>

<style>
  .contact {
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

  .contact-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
  }

  .contact-info {
    display: grid;
    gap: 2rem;
  }

  .info-item {
    background: white;
    padding: 1.5rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .info-item h3 {
    color: #667eea;
    margin-bottom: 0.5rem;
    font-size: 1.1rem;
  }

  .info-item p {
    color: #666;
    margin: 0;
  }

  .info-item a {
    color: #667eea;
    text-decoration: none;
  }

  .info-item a:hover {
    text-decoration: underline;
  }

  .contact-form {
    background: white;
    padding: 2rem;
    border-radius: 0.8rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .form-group {
    margin-bottom: 1.5rem;
  }

  .form-group label {
    display: block;
    margin-bottom: 0.5rem;
    color: #333;
    font-weight: 500;
  }

  .form-group input,
  .form-group textarea {
    width: 100%;
    padding: 0.8rem;
    border: 1px solid #ddd;
    border-radius: 0.5rem;
    font-family: inherit;
    font-size: 1rem;
    transition: border-color 0.3s;
  }

  .form-group input:focus,
  .form-group textarea:focus {
    outline: none;
    border-color: #667eea;
    box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
  }

  .btn-submit {
    width: 100%;
    padding: 0.8rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    border: none;
    border-radius: 0.5rem;
    font-weight: 600;
    font-size: 1rem;
    cursor: pointer;
    transition: all 0.3s;
  }

  .btn-submit:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 20px rgba(102, 126, 234, 0.3);
  }

  .success-message {
    background: #d4edda;
    color: #155724;
    padding: 1.5rem;
    border-radius: 0.5rem;
    text-align: center;
    font-weight: 500;
  }

  @media (max-width: 768px) {
    .contact {
      padding: 3rem 1rem;
    }

    h2 {
      font-size: 1.8rem;
    }

    .contact-content {
      grid-template-columns: 1fr;
      gap: 2rem;
    }
  }
</style>

