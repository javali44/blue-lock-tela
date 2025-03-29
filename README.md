local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")

-- Cria um Frame que cobre toda a tela
local screenFrame = Instance.new("Frame")
screenFrame.Size = UDim2.new(1, 0, 1, 0) -- Tamanho total da tela
screenFrame.Position = UDim2.new(0, 0, 0, 0) -- Posição no canto superior esquerdo
screenFrame.BackgroundColor3 = Color3.fromRGB(0, 0, 0) -- Cor de fundo (preto)
screenFrame.BackgroundTransparency = 0.5 -- Transparência do fundo
screenFrame.Parent = playerGui

-- Adiciona um efeito de esticar a tela
local function stretchScreen()
    screenFrame.Size = UDim2.new(1, 0, 1, 0)
end

-- Chama a função para esticar a tela
stretchScreen()
