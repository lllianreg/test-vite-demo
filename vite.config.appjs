import { defineConfig } from "vite";
import vue from "@vitejs/plugin-vue";
import { AntDesignVueResolver } from "unplugin-vue-components/resolvers";
import Components from "unplugin-vue-components/vite";

// https://vitejs.dev/config/
export default defineConfig({
  plugins: [
    vue(),
    Components({
      resolvers: [
        AntDesignVueResolver({
          exclude: ["AModal"],
        }),
      ],
      // include: [/[\\/]node_modules[\\/]easy-coms-vite/, /\.vue$/, /\.vue\?vue/],
      exclude: [
        /[\\/]node_modules[\\/]((?!easy-coms|easy-coms-vite\/).)/,
        /[\\/]\.git[\\/]/,
        /[\\/]\.nuxt[\\/]/,
      ],
    }),
  ],
  // server: {
  //   port: 8080,
  // },
});
