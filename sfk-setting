const setTranslateQuery = (lang) => {
    const render = (res) => res[0].map(r => r[0]).join('');
    Front.registerInlineQuery({
        url: `https://translate.googleapis.com/translate_a/single?client=gtx&sl=auto&tl=${lang}&dt=t&dt=bd&q=`,
        parseResult: res => [ render(JSON.parse(res.text)) ],
    });
};

setTranslateQuery('ru');
