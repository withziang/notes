# React and HTML note

- variable component attribute: `{...(dateValue ? { value: dateValue } : {})}`
- varibale style attribute ` ...(windowHeight < windowWidth ? {height: '65%'} : {width: '70%'})`
- Js function within HTML ```    {(() => {
                                    switch (selectedIndex) {
                                        case 0:
                                            return <SelectChessBoardBackground boardIndex={boardIndex} setBoardIndex={setBoardIndex} windowWidth={windowWidth}/>;
                                        case 1:
                                            return <GameMode/>;
                                        default:
                                            return <></>;
                                    }
                                })()} ```