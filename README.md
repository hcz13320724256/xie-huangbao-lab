# 蟹黄堡实验室 · Xie-Huangbao Laboratory

基于 [Greene Lab Website Template](https://github.com/greenelab/lab-website-template) 的课题组公开网站。原模板版权与 BSD-3-Clause 许可证保留在 LICENSE.md。

## 内容与更新

- 首页与栏目：index.md、research/、projects/、team/、contact/。
- 论文：_data/citations.yaml。保留原有题目、作者、年份、DOI 和贡献标注，不自动改写已有记录。
- 研究方向与项目：_data/lab.yaml。
- 成员个人页：_members/member-1.md 等；图片在 images/。
- 无在线登录、数据库写入或文件上传后台。通过 GitHub 编辑公开文件，提交后自动构建部署。
- 不要提交密码、密钥、.env、未公开论文或其他私人数据。

## 发布

在仓库 Settings → Pages 中将 Source 设为 GitHub Actions；推送 main 后工作流会构建 Jekyll 并发布 Pages。
在 GitHub Actions 的 “Build and deploy lab website” 中查看构建和部署结果。

当前配置的项目地址为 https://hcz13320724256.github.io/xie-huangbao-lab/ ，以上线后的实际 Pages 地址为准。
原域名没有在本版本中预先绑定；新地址验证通过后再配置自定义域名和 DNS。

## 数据保真

迁入 21 篇论文、4 个研究方向、2 个科研项目、1 个项目成果和 5 名成员。
内容沿用原网站公开资料；模板转换不等于重新核验论文或项目事实。缺失资料仍保留原有标注。
自动 ORCID、示例引用及定时同步暂未启用，避免模板样例或外部元数据覆盖已有作者贡献记录。
模板原有的初始化清理工作流已替换为提示步骤；不需要再运行它。Pull Request 只检查构建，不自动重写引用数据。

## 本地预览

需要 Ruby 和 Bundler。安装依赖后运行 `bundle exec jekyll serve --baseurl /xie-huangbao-lab`。
