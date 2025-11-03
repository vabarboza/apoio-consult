<template>
  <div class="box">
    <!-- Título do formulário -->
    <h2 class="title is-5 has-text-centered has-text-weight-bold">
      <p>ENTRE EM CONTATO</p>
    </h2>

    <form @submit.prevent="enviarEmail" ref="form">
      <!-- Nome -->
      <div class="field">
        <div class="control">
          <input 
            class="input" 
            type="text" 
            name="from_name" 
            v-model="nome" 
            placeholder="Nome" 
            required
          >
        </div>
      </div>

      <!-- E-mail -->
      <div class="field">
        <div class="control">
          <input 
            class="input" 
            type="email" 
            name="reply_to" 
            v-model="email" 
            placeholder="E-mail" 
            required
          >
        </div>
      </div>

      <!-- Assunto -->
      <div class="field">
        <label class="label">Assunto</label>
        <div class="control">
          <div class="select is-fullwidth">
            <select v-model="assunto" required>
              <option value="" disabled selected>Selecione uma opção</option>
              <option value="Orçamento">Orçamento</option>
              <option value="Dúvidas">Dúvidas</option>
            </select>
          </div>
        </div>
      </div>

      <!-- Mensagem -->
      <div class="field">
        <div class="control">
          <textarea 
            class="textarea" 
            name="message" 
            v-model="mensagem" 
            rows="4" 
            placeholder="Mensagem" 
            required
          ></textarea>
        </div>
      </div>

      <!-- Botão de envio -->
      <div class="field">
        <div class="control">
          <button class="button is-dark is-fullwidth" type="submit">
            ENVIAR
          </button>
        </div>
      </div>

      <!-- Feedback (opcional, apenas placeholders) -->
      <div v-if="enviado" class="notification is-success mt-2">
        Formulário enviado com sucesso!
      </div>
      <div v-if="falhou" class="notification is-danger mt-2">
        Falha ao enviar formulário!
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormIndex',
  data() {
    return {
      nome: '',
      email: '',
      assunto: '',
      mensagem: '',
      enviado: false,
      falhou: false
    };
  },
  methods: {
    enviarEmail() {
      // Placeholder para lógica futura de envio
      console.log("Enviar formulário:", {
        nome: this.nome,
        email: this.email,
        assunto: this.assunto,
        mensagem: this.mensagem
      });

      // Apenas simulação de envio
      this.enviado = true;
      this.falhou = false;

      // Limpar campos
      this.nome = '';
      this.email = '';
      this.assunto = '';
      this.mensagem = '';
    }
  }
};
</script>

<style scoped>
/* Ajustes opcionais */
.mt-2 {
  margin-top: 0.5rem;
}
</style>
