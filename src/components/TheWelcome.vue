<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'

const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>文档</template>

    Vue的
    <a href="https://vuejs.org/" target="_blank" rel="noopener">官方文档</a>
    提供了你入门所需的所有信息。
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>工具</template>

    这个项目使用
    <a href="https://vite.dev/guide/features.html" target="_blank" rel="noopener">Vite</a> 进行服务和打包。推荐的IDE设置是
    <a href="https://code.visualstudio.com/" target="_blank" rel="noopener">VSCode</a>
    +
    <a href="https://github.com/vuejs/language-tools" target="_blank" rel="noopener">Vue - 官方</a>。如果你需要测试你的组件和网页，可以查看
    <a href="https://vitest.dev/" target="_blank" rel="noopener">Vitest</a>
    和
    <a href="https://www.cypress.io/" target="_blank" rel="noopener">Cypress</a>
    /
    <a href="https://playwright.dev/" target="_blank" rel="noopener">Playwright</a>。

    <br />

    更多说明可以在
    <a href="javascript:void(0)" @click="openReadmeInEditor"><code>README.md</code></a
    >中找到。
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>生态系统</template>

    为你的项目获取官方工具和库：
    <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>,
    <a href="https://router.vuejs.org/" target="_blank" rel="noopener">Vue Router</a>,
    <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener">Vue Test Utils</a>，以及
    <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener">Vue Dev Tools</a>。如果你需要更多资源，我们建议访问
    <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">Awesome Vue</a>。
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>社区</template>

    遇到困难？在
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a>
    （我们的官方Discord服务器）上提问，或者访问
    <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener"
      >StackOverflow</a
    >。你还应该关注官方的
    <a href="https://bsky.app/profile/vuejs.org" target="_blank" rel="noopener">@vuejs.org</a>
    Bluesky账号或
    <a href="https://x.com/vuejs" target="_blank" rel="noopener">@vuejs</a>
    X账号，以获取Vue世界的最新消息。
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>支持Vue</template>

    作为一个独立项目，Vue依赖社区支持来维持其可持续性。你可以通过
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">成为赞助商</a>来帮助我们。
  </WelcomeItem>
</template>
