import { createContext, ReactNode } from "react";

//tipo de children
interface CountdownProviderPorps {
    children: ReactNode;
}


interface CountdownContextData {

}

const CountdownContext = createContext({} as CountdownContextData);

export function CountdownProvider({ children }: CountdownProviderPorps) {

    return (
        <CountdownContext.Provider value={{
            
        }}>
            {children}
        </CountdownContext.Provider>
    )

}
