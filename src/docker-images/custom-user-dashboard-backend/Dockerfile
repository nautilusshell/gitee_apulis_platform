FROM node:12

RUN mkdir -p /home/addon_custom_user_dasboard_backend
WORKDIR /home/addon_custom_user_dasboard_backend
RUN git clone https://gitee.com/apulis_contact/user-dashboard-backend.git /home/addon_custom_user_dasboard_backend
RUN yarn config set registry 'https://registry.npm.taobao.org'
RUN yarn
RUN yarn build

EXPOSE 5001

CMD ["yarn", "start:prod"]
