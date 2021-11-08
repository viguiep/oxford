Normalement, cela permet d'avoir la démo Streamlit accessible depuis www.qoqaq.com

PRINCIPE:
- Github Pages => index.html
- iframe dans index.html => renvoi vers le site de Streamlit https://share.streamlit.io/viguiep/streamlit_test/main/nlp.py
- creation d'un CNAME via Github Pages (fichier à la racine du répertoire, nommé CNAME, et contenant l'url de destination, ici www.qoqaq.com)
- dans Namebay (par exemple): Host = www, type = CNAME, priority = 10, hostname = viguiep.github.io.)

Remarque: un redirect dans Namebay vers un sous-répertoire (comme l'url de Streamlit) ne marche pas.

NLP test - 
Accessible at https://viguiep.github.io/oxford/

Point to https://share.streamlit.io/viguiep/streamlit_test/main/nlp.py
(which is a copy of https://github.com/viguiep/streamlit_test)

Github instructions
- configure external DNS: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site
- unpublish site: https://docs.github.com/en/pages/getting-started-with-github-pages/unpublishing-a-github-pages-site
