pragma solidity 0.5.12;

contract AcordoCooperacao {

string public nomeParteA;
string public nomeParteB;
address public chaveParteA;
address public chaveParteB;
string public objeto;
uint public parteAHorasVariaveis;
uint public parteBHorasVariaveis;

constructor(
    string memory _nomeParteA,
    string memory _nomeParteB,
    address _chaveParteA,
    address _chaveParteB,
    string memory _objeto)
public {
    
    nomeParteA = _nomeParteA;
    nomeParteB = _nomeParteB;
    chaveParteA = _chaveParteA;
    chaveParteB = _chaveParteB;
    objeto = _objeto;
}

function computarHorasTrabalhadas (uint parteHorasVariaveis)
public {
    require (msg.sender == chaveParteA || chaveParteB == msg.sender);
    if (msg.sender == chaveParteA) {
        parteAHorasVariaveis = parteAHorasVariaveis + parteHorasVariaveis;
    } else {
        parteBHorasVariaveis = parteBHorasVariaveis + parteHorasVariaveis;
    }
    
}
}
