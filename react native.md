``` bash
Boolean(!this.props.noArrow)
sceneConfigs: Navigator.SceneConfigs.PushFromRight //通过这个参数可以修改界面在导航时候切换的动画。
router.push(Routes.COMMON_PDF_READER, {
    title: item.name,
    passProps: {
        url: item.url,
    },
    sceneConfigs : Navigator.SceneConfigs.PushFromRight,
})
global.LOCAL_FUND_TYPE_LIST //类似window
item.annual_rate.split('.')[0]
parseFloat(item.collect_process, 10)
Array.isArray(fundInfo.yield)
router.push(Routes.USERLOGIN, {
    passProps: {
        fromRoute: router.currentRoute,
    }
});
<ITextInput
    textStyle = {[styles.textRemarkInput, styles.textAmount]}
    onChangeText = {(amount) => {
        this.setState({
            amount: amount
        });
    } }
    value={this.state.amount} />
router.resetTo(Routes.MAIN, {
    passProps: {
        selectedTab: 3
    }
});
let userBaseInfo = Object.assign(iResponseUser.responseData.data, {
    userToken: iResponse.responseData.user_token, // 登录token
    userMobile: this.state.mobile, // 用户手机号
});

<ITextInput
    textStyle = {[styles.textInput, {width: Base.layouts.vSeparations.v220}]}
    placeholder="点击搜索产品名称"
    onChangeText = {(fund_name_search) => {
        this.setState({
            fund_name_search: fund_name_search,
        });
        this._searchFundList(fund_name_search);
    } }
    onFocus = {() => {
        this.state.is_focus = true;
    } }
    value = {this.state.fund_name_search}
/>


var str = "我们都是好孩子";
undefined
str.split('都是');
["我们", "好孩子"]
<Text style = {styles.pullDownText}>
{itemArr[0]}
<Text style = {styles.pullDownTextColor}>{this.state.fund_name_search}</Text>
{itemArr[1]}
</Text>

var keys = Object.keys(params);
var o = {
    mobile: 13890890989,
    type: 'REGISTER',
    typeName: '注册',
}
undefined
Object.keys(o)
["mobile", "type", "typeName"]

Array.isArray(this.state.order_amount_detail) && Boolean(this.state.order_amount_detail.length) &&
this.state.order_amount_detail.map((detail, index, arr) => {
    return (
    <View key = {'detail' + index}>
    <View style={styles.item}>
    <Text>{detail.title}</Text>
    <Text>¥{detail.amount}万</Text>
    </View>
    {
        Boolean(index !== this.state.order_amount_detail.length - 1) &&
        <View style={[CommonStyle.lineStyle, styles.line]} />
    }
    </View>
    );
})

let newUserInfo = Object.assign(this.state.userInfo, { address: this.state.address });
// 更新本地用户数据
CM.post(new IRequest(APIConstants.UPDATE_USER_INFO, newUserInfo, this), () => {
    router.replacePreviousAndPop(Routes.USERDATA);
});

******************************************************************
var REQUEST_PREFIX = AppInfo.API_HOST+ServiceAPI.verifyCode;

class ValidCode extends Component {

    constructor(...props) {
    super(...props);

    this.state = {
    codeUri : REQUEST_PREFIX+'?key='+this.props.type+'&t='+(new Date().getTime())
};
}

    _refreshCode() {
    this.setState({
    codeUri : REQUEST_PREFIX+'?key='+this.props.type+'&t='+(new Date().getTime())
});
}

    render() {
    return (
    <View style={styles.wapper}>
    <Image style={styles.code} source={{uri: this.state.codeUri}} resizeMode='stretch'/>
    <TouchableOpacity
    activeOpacity={1}
    type = {this.props.type}
    onPress={this._refreshCode.bind(this)}
    >
    <Text style={styles.refreshText}>刷新字符</Text>
    </TouchableOpacity>
    </View>
    );
    }
}
```