# react-props
하위 컴포넌트로 data 전달하기
```jsx
 <div className="layout">
     <FirstChild data={leftCount}/>
     <SecondChild setLeft={setLeftCount}
         setRight={setRightCount}
         resetData={resetData}/>
     <ThirdChild data={rightCount}/>
 </div>
 ```
 
 부모 컴포넌트로부터 데이터 받기
 ```jsx
 const FirstChild =(props)=>{
    console.log(`자식1 ${props.data}`);
    return(
        <div className="first">
            <p>자식1 컴포넌트</p>
            <p>(카운터:{props.data})</p>
        </div>
    )
};
```
